# Sistema de Ventas

Este proyecto es una aplicación web para la gestión de ventas, clientes, productos y reportes. Permite administrar inventario, realizar ventas, generar facturas y visualizar estadísticas.

## Tecnologías utilizadas

- **Lenguajes:**  
    - PHP  
    - JavaScript  
    - HTML  
    - CSS

- **Frameworks y Librerías:**  
    - Bootstrap (diseño responsivo)  
    - jQuery (interactividad)  
    - Font Awesome (iconos)  
    - MySQL (base de datos)

## Archivo `.htaccess`

El archivo `.htaccess` se utiliza para configurar reglas en el servidor Apache, como:

- Redirecciones de URL.
- Protección de directorios.
- Configuración de permisos.
- Habilitar URLs amigables (mod_rewrite).
- Mejorar la seguridad del sitio.

`Options -Indexes`

 * Evita que los usuarios vean el contenido de las carpetas si no hay un archivo index.

`RewriteEngine On`

 * Activa el sistema de reescritura de URLs.


`RewriteCond %{REQUEST_FILENAME} !-f`

 * Si la URL no corresponde a un archivo existente...


`RewriteCond %{REQUEST_FILENAME} !-d`

 * verifica si la URL no corresponde a un directorio existente...



`RewriteRule ^(.*)$ index.php?/$1 [L]`

 * Si no se encontraron archivos o directorios, redirige todo a index.php, pasando la URL como parámetro.

En este proyecto, `.htaccess` ayuda a gestionar el acceso y la estructura de las URLs, facilitando la navegación y protegiendo recursos sensibles.
