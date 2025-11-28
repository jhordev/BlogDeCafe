# Documentación del proyecto BlogDeCafé

## Descripción general
BlogDeCafé es un sitio estático en español dedicado a compartir contenido sobre café, cursos y talleres, así como un canal de contacto para la comunidad. Todas las páginas comparten una cabecera con imagen de fondo, el logotipo "BlogDeCafé" y una navegación primaria hacia las secciones principales.

## Estructura de archivos
- `index.html`: Página de inicio con listados de entradas destacadas y un resumen de cursos en la barra lateral.
- `nosotros.html`: Sección informativa sobre la historia y el enfoque del blog.
- `cursos.html`: Catálogo de próximos cursos y talleres con precio, cupo y descripciones.
- `entrada.html`: Plantilla de detalle para las entradas del blog.
- `contacto.html`: Formulario para que los usuarios envíen su nombre, correo y mensaje.
- `css/normalize.css`: Restablece estilos predeterminados del navegador.
- `css/style.css`: Hoja de estilos principal del sitio.
- `img/`: Carpeta de imágenes (banner, cursos, entradas, formulario de contacto y fotos institucionales).

## Estructura y componentes de las páginas
- **Cabecera común**: Bloque `.header` con imagen de fondo (`img/banner.jpg`), eslogan "Blog de café con consejos y cursos" y navegación (`.navegacion`) hacia Nosotros, Cursos y Contacto.
- **Páginas de contenido**:
  - Inicio (`index.html`): Usa el contenedor principal `.contenido-principal` para distribuir la columna de blog y la barra lateral mediante grid. Cada artículo `.entrada` incluye imagen, título, párrafo y botón "Leer Entrada".
  - Nosotros (`nosotros.html`): Sección `.sobre-nosotros` con disposición en dos columnas para imagen y texto descriptivo.
  - Cursos (`cursos.html`): Lista de bloques `.curso` que combinan imágenes y detalles del taller; muestran precio y tamaño del grupo.
  - Entrada (`entrada.html`): Muestra la imagen de la entrada y varios párrafos con la clase `.texto-parrafo`.
  - Contacto (`contacto.html`): Fondo ilustrativo (`.contacto-bg`) seguido de un formulario `.formulario` con campos alineados mediante `.campo`, `.campo__label` y `.campo__field`.

## Estilos y tipografías
- Tipografías importadas desde Google Fonts: **PT Sans** para encabezados y **Open Sans** para párrafos.
- Paleta de colores centralizada en variables CSS (`--primario`, `--gris`, `--blanco`, `--negro`).
- Diseño responsivo a partir de 768px con grids y flexbox para la barra de navegación, la disposición principal, la sección Sobre Nosotros y los listados de cursos.
- Botones reutilizables `.boton` con variantes `.boton--primario` (fondo negro) y `.boton--secundario` (color primario).

## Recursos estáticos
- Las imágenes se encuentran en `img/` y se referencian desde las páginas mediante rutas relativas.
- El banner principal (`img/banner.jpg`) se aplica como `background-image` en `.header` y se adapta a diferentes tamaños con `background-size: cover`.

## Ejecución local
Al ser un sitio estático, no requiere dependencias ni servidor específico. Para revisarlo localmente:
1. Clona o descarga el repositorio.
2. Abre `index.html` en tu navegador preferido.
3. Navega por las secciones mediante la barra superior.

## Flujo de contribución sugerido
1. Crea una nueva rama descriptiva a partir de `work`.
2. Realiza cambios en HTML, CSS o imágenes según corresponda.
3. Verifica la visualización local abriendo los archivos `.html` en el navegador.
4. Envía un Pull Request con un resumen claro de los cambios y captura de pantalla si hay modificaciones visuales.
