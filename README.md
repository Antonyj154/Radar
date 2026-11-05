# Radar diario

App web para ver los hallazgos del Radar diario guardados en Airtable (base Marketing, tablas "radar general", "daily" y "Topicos").

## Publicarla gratis con GitHub Pages
1. Crea una cuenta en github.com (si no tienes).
2. Crea un repositorio nuevo, por ejemplo `radar`. Puede ser público o privado (con cuenta gratuita, Pages funciona en repositorios públicos).
3. En el repositorio: **Add file > Upload files** y sube todo el contenido de esta carpeta (index.html, manifest.webmanifest, sw.js, los íconos y la carpeta logos).
4. Ve a **Settings > Pages**, en "Branch" elige `main` y la carpeta `/ (root)`, y guarda.
5. En 1 o 2 minutos tendrás el link: `https://TU-USUARIO.github.io/radar/`

El código no contiene tu token: lo escribes dentro de la app y queda guardado solo en tu dispositivo.

## Conectar Airtable
La base (Marketing) y las tablas ya vienen fijas en el código. El token NO está en el código: se pega una sola vez por dispositivo.
- Opción 1: abre la app y pega el token en la pantalla "Conecta Radar".
- Opción 2: abre una vez el enlace `https://TU-USUARIO.github.io/radar/#token=TU_TOKEN`. La app guarda el token y lo borra de la barra de direcciones.

El token necesita acceso a la base Marketing con los permisos `data.records:read` y `data.records:write`.

## Logos
Los logos de cada plataforma vienen incluidos dentro de index.html, así que funcionan incluso sin internet.

## Si cambian los nombres de los campos
Edita los bloques `const AIRTABLE` y `const F` al inicio del script en index.html.
