# Aula Web — código fuente para Vercel

Versión actual: referencias específicas de MDN en las 21 fichas HTML y las 21 fichas CSS, menú sin el bloque HTML + CSS / La Litoral, interfaz actualizada e iconos Bootstrap Icons.

## Archivos

- dist/index.html: estructura y navegación.
- dist/style.css: colores, componentes, transiciones, scrolls e iconos.
- dist/app.js: contenidos, ejemplos, navegación y lectura en inglés.
- dist/fonts/bootstrap-icons.woff2: fuente de iconos alojada localmente.
- dist/fonts/bootstrap-icons-LICENSE.txt: licencia de Bootstrap Icons.
- vercel.json: configuración para desplegar el sitio sin compilación.

## 1. Descargar y descomprimir

Descomprime el ZIP. No subas el ZIP al repositorio: sube sus archivos descomprimidos.

## 2. Crear o abrir un repositorio en GitHub

Para un repositorio nuevo, pulsa New repository y asigna un nombre, por ejemplo aula-web.
Puedes elegir público o privado. Si utilizas un repositorio existente, conserva sus otros archivos y coloca este proyecto en una carpeta independiente cuando ya contenga otra aplicación.

## 3. Subir los archivos

En GitHub elige Add file > Upload files (en un repositorio vacío, uploading an existing file).
Arrastra la carpeta dist completa y los archivos vercel.json y README.md.
Pulsa Commit changes.

La raíz del proyecto debe contener dist, README.md y vercel.json. Dentro de dist debe estar index.html. No subas .git, .openai, credenciales ni archivos de configuración de Sites.

## 4. Importar en Vercel

Abre https://vercel.com/new e inicia sesión.
Conecta GitHub y autoriza el acceso al repositorio elegido.
Busca el repositorio y pulsa Import.

## 5. Revisar la configuración

- Framework Preset: Other.
- Root Directory: raíz del repositorio; si el proyecto está en una subcarpeta, selecciona esa subcarpeta.
- Build Command: vacío (activa Override si hace falta para dejarlo vacío).
- Install Command: vacío.
- Output Directory: dist.
- Variables de entorno: no requiere ninguna.

vercel.json ya define la carpeta de salida y los comandos vacíos.

## 6. Publicar y comprobar

Pulsa Deploy. Cuando termine, abre la dirección que Vercel asigne.
Comprueba las seis secciones, los iconos y el audio desde un equipo y un móvil.
La lectura en inglés usa las voces del navegador o dispositivo. Requiere pulsar el altavoz; no usa una API de pago.

## 7. Actualizar

Modifica los archivos y guarda los cambios en la rama de producción del repositorio.
Vercel puede publicar automáticamente los cambios de esa rama.

Para editar contenido cambia dist/app.js; para editar el diseño cambia dist/style.css; para editar la estructura cambia dist/index.html.

## Vista local

Abre dist/index.html en un navegador. Si prefieres un servidor local, desde la raíz ejecuta python -m http.server 8080 --directory dist y visita http://localhost:8080.

## Referencias

https://vercel.com/docs/builds/configure-a-build
https://vercel.com/docs/project-configuration
https://vercel.com/docs/git
https://icons.getbootstrap.com/
