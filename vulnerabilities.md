# Vulnerabilidades Críticas Identificadas
-------------------------GPSMapsApp---------------------------------
1. Comunicación HTTP insegura
La aplicación se comunica utilizando HTTP en lugar de HTTPS, lo que permite que los datos puedan ser interceptados por hackers o atacantes en ataques de tipo Man-in-the-Middle (MITM).
SOLUCION: Cambiar todas las comunicaciones a HTTPS para asegurar que los datos en tránsito estén protegidos.
------------------------------------------------------------------------------------------------------------
2. Debugging habilitado:
La opción `android:debuggable=true` está habilitada en el archivo `AndroidManifest.xml`, lo que facilita a los hackers puedan depurar la aplicación en un entorno de producción.
SOLUCION: Deshabilitar el modo de depuración en el archivo `AndroidManifest.xml` para las versiones de producción. La opción debería ser `android:debuggable=false` para evitar que los hackers depuren la app.
------------------------------------------------------------------------------------------------------------
3. Permisos peligrosos:
La aplicación solicita permisos de acceso a la ubicación precisa (`ACCESS_FINE_LOCATION`) y aproximada (`ACCESS_COARSE_LOCATION`). Estos permisos podrían exponer la privacidad de los usuarios si no se gestionan adecuadamente.
SOLUCION: Eliminar los permisos innecesarios en el archivo `AndroidManifest.xml` si la app no necesita acceso a la ubicación. En caso de requerir estos permisos, proporcionar una justificación clara a los usuario, debido a que la app es un mapa y ocupa la ubicacion y garantizar que los datos de ubicación estén protegidos.
------------------------------------------------------------------------------------------------------------
4. Certificado de depuración:
La aplicación está firmada con un certificado de depuración, lo que no es adecuado para versiones de producción, ya que no proporciona seguridad criptográfica suficiente.
SOLUCION: Firmar la aplicación con un certificado de producción antes de su lanzamiento para asegurar la autenticidad de la app y evitar que sea modificada por terceros.
------------------------------------------------------------------------------------------------------------
5. Uso de dependencias desactualizadas:
MobSF detectó que la aplicación está utilizando dependencias que tienen vulnerabilidades conocidas. Mantener bibliotecas desactualizadas podría permitir a los hackers explotar esas vulnerabilidades.
SOLUCION: Actualizar todas las dependencias de la aplicación a sus versiones más recientes y seguras.

-------------------------GPSMapsApp---------------------------------


