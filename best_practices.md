# Mejores Prácticas de Seguridad Implementadas
-------------------------GPSMapsApp---------------------------------
1. Uso de HTTPS en comunicaciones de red:
Todas las comunicaciones de red de la aplicación se han configurado para utilizar HTTPS, garantizando que los datos transferidos estén encriptados y protegidos contra ataques de tipo Man-in-the-Middle (MITM).
IMPACTO QUE TIENE EN LA SEGURIDAD: El uso de HTTPS asegura que los datos no puedan ser interceptados ni modificados por atacantes.
------------------------------------------------------------------------------------------------------------
2. Deshabilitar el debugging en producción:
La opción `android:debuggable` fue deshabilitada en el archivo `AndroidManifest.xml` para versiones de producción, asegurando que la app no pueda ser depurada en dispositivos de los usuarios.
IMPACTO QUE TIENE EN LA SEGURIDAD: Esto previene que atacantes puedan conectar herramientas de depuración a la aplicación y extraer información confidencial o modificar su comportamiento.
------------------------------------------------------------------------------------------------------------
3. Eliminar permisos innecesarios:
Los permisos de ubicación (`ACCESS_FINE_LOCATION` y `ACCESS_COARSE_LOCATION`) fueron revisados y eliminados en caso de no ser absolutamente necesarios para la funcionalidad de la app.
IMPACTO QUE TIENE EN LA SEGURIDAD: Esto protege la privacidad del usuario, asegurando que la aplicación no tenga acceso a información sensible como la ubicación del dispositivo si no es necesario.
------------------------------------------------------------------------------------------------------------
4. Uso de certificado de producción:
La aplicación fue firmada con un certificado de producción en lugar de un certificado de depuración.
IMPACTO QUE TIENE EN LA SEGURIDAD: Esto garantiza que la aplicación sea auténtica y no haya sido modificada por terceros antes de ser distribuida a los usuarios finales.
------------------------------------------------------------------------------------------------------------
5. Actualización de dependencias:
Todas las dependencias de la aplicación fueron actualizadas a sus versiones más recientes y seguras.
IMPACTO QUE TIENE EN LA SEGURIDAD: Actualizar las dependencias mitiga las vulnerabilidades conocidas en versiones antiguas de bibliotecas de terceros, mejorando la seguridad general de la aplicación.
-------------------------GPSMapsApp---------------------------------