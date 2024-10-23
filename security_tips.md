# Tips de seguridad.
-------------------------------GPGMapsApp-----------------------------------
1. Deshabilitar el debugging en producción:
   Se deshabilitó la opción de debugging en el archivo AndroidManifest.xml para evitar que la app sea depurada en dispositivos de los usuarios.
   Impacto en la seguridad: Esto impide que atacantes puedan conectarse a la app con herramientas de depuración y modificar su comportamiento o extraer información sensible.
------------------------------------------------------------------------------------------------------------
2. Uso de HTTPS para todas las comunicaciones:
   Todas las comunicaciones de la aplicación con la API de Google Maps se realizan utilizando HTTPS, lo que garantiza que los datos transmitidos estén encriptados.
   Impacto en la seguridad: Esto protege contra ataques de tipo Man-in-the-Middle (MITM), asegurando la confidencialidad de los datos durante el tránsito.
------------------------------------------------------------------------------------------------------------
3. Permisos mínimos necesarios:
   Se revisaron y limitaron los permisos a los estrictamente necesarios: acceso a la ubicación precisa y aproximada, además del acceso a internet.
   Impacto en la seguridad: Esto reduce los riesgos de exposición de información sensible al limitar el acceso de la app a solo lo esencial.
-------------------------------GPGMapsApp-----------------------------------
