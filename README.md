# SOMOS Torreón: sitio web

Sitio del Comité Municipal de SOMOS en Torreón, Coahuila. Las noticias se editan desde un panel (Pages CMS), sin tocar código.

## Qué hay en esta carpeta

| Archivo o carpeta | Para qué sirve |
|---|---|
| `index.html` | La página completa |
| `img/` | Logos y foto del equipo juvenil |
| `content/noticias.json` | Las noticias. Se edita desde el panel |
| `media/` | Aquí se guardan las fotos que se suben desde el panel |
| `.pages.yml` | Configuración del panel de noticias |

## Puesta en marcha (una sola vez)

### 1. Subir a GitHub
1. En GitHub, crea un repositorio nuevo llamado `somos-torreon`.
2. Entra al repositorio y elige **Add file → Upload files**.
3. Arrastra **el contenido** de esta carpeta (no la carpeta misma): `index.html`, `img`, `content`, `media`, `.pages.yml` y este `README.md`. Luego da clic en **Commit changes**.
4. Revisa que aparezca `.pages.yml` en la lista. Si no aparece (en Mac los archivos que empiezan con punto vienen ocultos; se muestran con Cmd + Shift + .), créalo con **Add file → Create new file**, nómbralo `.pages.yml` y pega su contenido.

### 2. Conectar con Netlify
1. En Netlify: **Add new site → Import an existing project → GitHub** y elige `somos-torreon`.
2. Deja vacío el comando de compilación (build command) y como carpeta de publicación deja la raíz. Da clic en **Deploy**.
3. En la configuración del sitio cámbiale el nombre, por ejemplo `somos-torreon`.
4. Desde ahora, cada cambio en GitHub se publica solo. El sitio que subiste con Drop ya no hace falta.

### 3. Activar el panel de noticias
1. Entra a **app.pagescms.org** e inicia sesión con GitHub.
2. Autoriza a Pages CMS para el repositorio `somos-torreon`.
3. Abre el repositorio: en el menú aparece **Noticias** con el formulario listo.
4. Invita a la persona del partido por correo desde la sección de colaboradores del proyecto. No necesita cuenta de GitHub.

## Cómo publicar una noticia (para la persona encargada)
1. Entra a **app.pagescms.org** con el correo con el que te invitaron.
2. Abre **Noticias** y agrega una nueva entrada.
3. Llena el formulario: título, imagen, categoría, fecha, resumen, contenido y autor. En el contenido, separa cada párrafo con una línea en blanco.
4. Deja apagado "¿Es noticia de ejemplo?".
5. Da clic en **Guardar**. En uno o dos minutos la noticia aparece en la página.

Para corregir o borrar una noticia, ábrela en el panel, cámbiala o elimínala y guarda.

## Secciones que se editan desde el panel
- **Noticias**: la página muestra las más recientes y un botón "Ver más noticias".
- **Actividades (Torreón)**: se agrupan solas por mes.
- **Actividades SOMOS Impacto**: se ven las 3 más recientes; las anteriores quedan en "Ver actividades anteriores".
- **Próximos eventos**: si no tiene fecha dice "Fechas por definir"; los eventos pasados se ocultan solos.
- **Galería SOMOS Impacto**: las fotos agregadas al final salen primero; con muchas fotos aparece "Ver más fotos".
