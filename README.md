# Mr. Trompito | Alquiler de Maquinaria, Mudanzas y Fletes

Sitio web desarrollado para **Mr. Trompito**, un emprendimiento familiar dedicado al alquiler de maquinaria y herramientas para la construcción, además de ofrecer servicios de mudanzas y fletes en Buenos Aires, Argentina.

El proyecto tiene como objetivo brindar una plataforma moderna, intuitiva y adaptable a distintos dispositivos, donde los usuarios puedan conocer los servicios disponibles, explorar el catálogo de maquinaria y solicitar presupuestos de manera sencilla.

## Demo del proyecto

**[Ver sitio web en GitHub Pages](https://agxs-tomassini.github.io/Mr-Trompito---Etapa-2/)**

**[Ver repositorio en GitHub](https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2)**

## Tecnologías utilizadas

- **HTML5:** estructura semántica y organización del contenido.
- **CSS3:** estilos personalizados, animaciones y efectos visuales.
- **Sass (SCSS):** organización modular de estilos mediante partials, variables, mixins y nesting.
- **Bootstrap 5:** sistema de grillas, componentes reutilizables y diseño responsive.
- **Bootstrap Icons:** iconografía para navegación, servicios y elementos de la interfaz.
- **Flexbox y CSS Grid:** distribución y alineación de elementos.
- **Git y GitHub:** control de versiones y almacenamiento del código.
- **GitHub Pages:** publicación del sitio web.
- **npm:** gestión de dependencias y ejecución de Sass.

## Páginas del sitio

### 1. Inicio (`index.html`)

Página principal con la presentación del emprendimiento, sus servicios destacados, información sobre maquinaria y una galería de imágenes implementada con el componente Carousel de Bootstrap.

### 2. Servicios (`pages/servicios.html`)

Catálogo de maquinaria, herramientas y equipos disponibles para alquiler.

Incluye tarjetas con información de cada equipo, imágenes o elementos visuales de referencia y enlaces para solicitar presupuestos.

### 3. Nosotros (`pages/nosotros.html`)

Sección destinada a presentar el emprendimiento, su actividad y la información institucional de Mr. Trompito.

### 4. Preguntas frecuentes (`pages/faq.html`)

Sección de consultas habituales, organizada mediante un Accordion de Bootstrap para facilitar la lectura y navegación.

### 5. Cotizador (`pages/cotizador.html`)

Página con formularios para solicitar presupuestos relacionados con:

- Alquiler de maquinaria y herramientas.
- Servicios de mudanzas, fletes y traslados.

Los formularios están organizados mediante el sistema de grillas de Bootstrap, con una distribución adaptable a dispositivos móviles y de escritorio.

## Diseño responsive y experiencia de usuario

El sitio está desarrollado con un enfoque adaptable a diferentes tamaños de pantalla.

Se priorizaron los siguientes aspectos:

- Navegación clara mediante un Navbar responsive.
- Diseño Mobile First.
- Uso de Flexbox y CSS Grid.
- Componentes visuales consistentes.
- Estados interactivos para botones, enlaces y formularios.
- Organización accesible del contenido mediante HTML semántico.
- Formularios y tarjetas adaptables a diferentes resoluciones.

## Arquitectura de estilos con SCSS

Los estilos del proyecto fueron refactorizados utilizando **Sass con sintaxis SCSS**, con el objetivo de mejorar la organización del código, facilitar su mantenimiento y reutilizar propiedades comunes.

La carpeta `scss/` se divide en cuatro directorios principales:

### `utilities/`

Contiene los recursos reutilizables de Sass:

- `_variables.scss`: colores, tipografías, bordes, sombras y otros valores de diseño.
- `_mixins.scss`: mixins para reutilizar configuraciones responsive.

### `base/`

Contiene los estilos generales del proyecto:

- `_base.scss`: reset, estilos globales, contenido principal y elementos generales.
- `_tipografia.scss`: configuración de títulos, párrafos y tipografía responsive.

### `layout/`

Contiene los estilos de las secciones estructurales:

- `_header.scss`: encabezado y logotipo.
- `_nav.scss`: navegación principal y menú responsive.
- `_footer.scss`: pie de página, redes sociales y newsletter.

### `components/`

Contiene los estilos de los componentes de la interfaz:

- `_buttons.scss`: botones y acceso flotante a WhatsApp.
- `_cards.scss`: tarjetas del catálogo de servicios.
- `_forms.scss`: formularios y Cotizador.
- `_carousel.scss`: galería de imágenes de Inicio.
- `_accordion.scss`: preguntas frecuentes.
- `_home.scss`: secciones específicas de la página de Inicio.

### Archivo maestro

El archivo `scss/main.scss` centraliza la importación de los partials mediante directivas `@use`.

Sass compila estos archivos y genera `css/main.css`, que es la hoja de estilos utilizada por las páginas HTML.

## Instalación y ejecución local

Para trabajar con el proyecto de manera local:

**1. Clonar el repositorio**

`git clone https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2.git`

**2. Ingresar a la carpeta del proyecto**

`cd Mr-Trompito---Etapa-2`

**3. Instalar las dependencias**

`npm install`

**4. Compilar los estilos SCSS**

Para generar el archivo CSS una sola vez:

`npx sass scss/main.scss css/main.css`

Para recompilar automáticamente al guardar modificaciones:

`npx sass --watch scss/main.scss:css/main.css`

**5. Abrir el sitio**

Abrir `index.html` en el navegador o utilizar una extensión de servidor local, como Live Server de Visual Studio Code.

**Importante:** los estilos deben modificarse desde los archivos SCSS. El archivo `css/main.css` se genera automáticamente y no debe editarse manualmente.

## Estado del proyecto

**Etapa 2 — Desarrollo Frontend**

En esta etapa se trabajó en:

- Desarrollo y organización de las cinco páginas HTML.
- Implementación de componentes Bootstrap.
- Diseño responsive con Flexbox y CSS Grid.
- Desarrollo de un catálogo de maquinaria.
- Organización de formularios de solicitud de presupuestos.
- Personalización del Carousel y del Accordion.
- Refactorización de CSS a SCSS.
- Incorporación de variables, mixins, nesting y partials.
- Publicación y actualización del proyecto mediante GitHub Pages.

El proyecto podrá ampliarse en futuras etapas con nuevas funcionalidades y mejoras.

## Autor

**Agustín Tomassini**

Estudiante de Tecnicatura en Informática y formación en Desarrollo Full Stack.

- **GitHub:** [@agxs-tomassini](https://github.com/agxs-tomassini)
- **Repositorio:** [Mr. Trompito – Etapa 2](https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2)

---

Desarrollado por **Agustín Tomassini** como parte de su formación y práctica en desarrollo web.