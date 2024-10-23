# GPSMapApp #

# Descripción 
Este proyecto es una aplicación Android que utiliza la API de Google Maps para mostrar la ubicación del usuario en tiempo real. Se han implementado medidas de seguridad para proteger contra vulnerabilidades comunes, garantizando que la aplicación sea segura en producción.

## Vulnerabilidades Identificadas 
- Comunicación no segura (uso de HTTP)
- Debugging habilitado en versiones de producción
- Permisos innecesarios o excesivos

## Mejoras Implementadas 
- Deshabilitar debugging en el archivo `AndroidManifest.xml`
- Uso de HTTPS para todas las comunicaciones de red
- Revisión y eliminación de permisos innecesarios

## Documentación 
- [Vulnerabilidades](vulnerabilities.md) 
- [Best Practices](best_practices.md) 
- [Security Tips](security_tips.md) 
- [Security Improvement Program](security_improvement_program.md) 

## Cómo Ejecutar la Aplicación de Forma Segura 
1. Clonar el repositorio.
2. Importar el proyecto en Android Studio.
3. Ejecutar la aplicación en un dispositivo o emulador con los permisos de ubicación necesarios habilitados.
4. Asegurarse de que la aplicación está firmada con un certificado de producción y que no tiene debugging habilitado.

## Reporte de Vulnerabilidades 
El reporte detallado de las pruebas de vulnerabilidad realizadas se encuentra en el archivo `ReporteVulnerabilidad.pdf`.
