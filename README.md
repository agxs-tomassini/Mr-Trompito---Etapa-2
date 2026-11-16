
# Mr. Trompito | Alquiler de Maquinaria, Mudanzas y Fletes

Sitio web desarrollado para **Mr. Trompito**, un emprendimiento familiar dedicado al alquiler de maquinaria y herramientas para la construcción, además de ofrecer servicios de mudanzas y fletes en Buenos Aires, Argentina.

El proyecto tiene como objetivo ofrecer una plataforma moderna, intuitiva y adaptable a distintos dispositivos, donde los usuarios puedan conocer los servicios, explorar el catálogo y consultar cómo solicitar un presupuesto.

## Demo del proyecto

**[Ver sitio web en Netlify](https://mr-trompito.netlify.app/)**

**[Ver repositorio en GitHub](https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2)**


## Tecnologías utilizadas

- **HTML5:** estructura semántica y organización del contenido.
- **CSS3:** estilos personalizados, transiciones y efectos visuales.
- **Sass (SCSS):** estilos modulares mediante variables, mixins, anidamiento, `@extend`, partials y `@use`.
- **Bootstrap 5.3.3:** sistema de grillas, Navbar responsive, Carousel, Accordion y formularios.
- **Bootstrap Icons:** iconografía para navegación, servicios y elementos de la interfaz.
- **Animate.css:** animaciones de entrada en los títulos principales.
- **Flexbox y CSS Grid:** distribución y alineación de secciones, paneles y tarjetas.
- **Google Fonts:** Barlow Condensed, Noto Sans y Petit Formal Script.
- **Git y GitHub:** control de versiones y alojamiento del código fuente.
- **Netlify:** publicación del sitio web estático.
- **npm:** gestión de dependencias y ejecución de Sass.

## Páginas del sitio

### 1. Inicio (`index.html`)

Página principal con un Hero que presenta el emprendimiento, imágenes de maquinaria y mudanzas, tarjetas de confianza, servicios destacados, galería de imágenes mediante el Carousel de Bootstrap y un enlace para conocer la historia de Mr. Trompito.

### 2. Servicios (`pages/servicios.html`)

Catálogo de maquinaria, herramientas y servicios de mudanzas y fletes, organizado con CSS Grid y adaptado a distintos tamaños de pantalla.

Incluye tarjetas con descripciones, fotografías o indicadores para imágenes pendientes y enlaces al Cotizador.

### 3. Nosotros (`pages/nosotros.html`)

Sección dedicada a la historia del emprendimiento, con una presentación acompañada por la fotografía del vehículo de trabajo, una línea de tiempo de tres etapas y un panel con los valores de puntualidad, seriedad y cuidado.

### 4. Preguntas frecuentes (`pages/faq.html`)

Consultas habituales sobre alquileres, zonas de cobertura y medios de pago, organizadas mediante un Accordion interactivo de Bootstrap.

### 5. Cotizador (`pages/cotizador.html`)

Página con dos formularios diferenciados para consultas relacionadas con:

- Alquiler de maquinaria y herramientas.
- Mudanzas, fletes y traslados.

Los formularios cuentan con campos obligatorios, etiquetas asociadas y una distribución responsive con Bootstrap y CSS Grid. **En esta versión son demostrativos y no envían datos a un servicio externo.**

## Diseño responsive y experiencia de usuario

El sitio fue rediseñado con una identidad visual consistente y una distribución adaptable a celulares, tablets y computadoras.

Se priorizaron los siguientes aspectos:

- Navegación clara mediante un Navbar responsive con menú desplegable en dispositivos móviles.
- Uso de Flexbox, CSS Grid y breakpoints compatibles con Bootstrap.
- Hero de Inicio con dos fotografías y contenido destacado.
- Tarjetas de catálogo, servicios y confianza con tamaños y espaciados adaptables.
- Carrusel con navegación manual mediante flechas e indicadores.
- Estados interactivos para botones, enlaces y formularios.
- HTML semántico, textos alternativos, foco visible y atributos ARIA en componentes que lo requieren.
- Reglas `prefers-reduced-motion` para respetar la preferencia de reducir animaciones.

La identidad visual utiliza una paleta de **azul marino (`#0b1f3b`), azul (`#2563eb`), celeste (`#60a5fa`) y fondos claros**, con detalles decorativos en **naranja (`#e75319`)**.

## Arquitectura de estilos con SCSS

Los estilos fueron organizados utilizando **Sass con sintaxis SCSS**, para facilitar el mantenimiento, evitar repeticiones y reutilizar configuraciones comunes.

La carpeta `scss/` se divide en cuatro directorios principales:

### `utilities/`

Contiene los recursos reutilizables de Sass:

- `_variables.scss`: paleta de colores, tipografías y variables auxiliares.
- `_mixins.scss`: mixins para breakpoints y reglas responsive reutilizables.

### `base/`

Contiene los estilos generales del proyecto:

- `_base.scss`: reset, estilos globales y elementos generales.
- `_tipografia.scss`: configuración de títulos, párrafos y tipografías destacadas.

### `layout/`

Contiene los estilos de las secciones estructurales:

- `_header.scss`: encabezado y logotipo.
- `_nav.scss`: navegación principal y menú responsive.
- `_footer.scss`: pie de página, redes sociales y newsletter.

### `components/`

Contiene los estilos de los componentes de la interfaz:

- `_buttons.scss`: botones de cotización y acceso flotante a WhatsApp.
- `_cards.scss`: tarjetas del catálogo de servicios.
- `_forms.scss`: formularios del Cotizador.
- `_carousel.scss`: galería de imágenes de Inicio.
- `_accordion.scss`: preguntas frecuentes.
- `_home.scss`: secciones específicas de la página Inicio.
- `_nosotros.scss`: Hero, trayectoria y compromiso de la página Nosotros.

### Archivo maestro

El archivo `scss/main.scss` centraliza la carga de los módulos mediante directivas `@use`.

Sass compila estos archivos y genera **`styles/main.css`**, que es la hoja de estilos utilizada por las páginas HTML.

## Instalación y ejecución local

Para trabajar con el proyecto de manera local:

**1. Clonar el repositorio**

```bash
git clone https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2.git
```

**2. Ingresar a la carpeta del proyecto**

```bash
cd Mr-Trompito---Etapa-2
```

**3. Instalar las dependencias**

```bash
npm install
```

**4. Compilar los estilos SCSS**

Para generar el archivo CSS una sola vez:

```bash
npx sass scss/main.scss styles/main.css --no-source-map
```

Para recompilar automáticamente al guardar modificaciones:

```bash
npx sass --watch scss/main.scss:styles/main.css
```

**5. Abrir el sitio**

Abrir `index.html` en el navegador o utilizar una extensión de servidor local, como Live Server de Visual Studio Code.

**Importante:** los estilos deben modificarse desde los archivos SCSS. El archivo `styles/main.css` se genera mediante Sass y no debe editarse manualmente.

## Estado del proyecto

**Proyecto Frontend — Versión publicada en Netlify**

En esta versión se desarrollaron y revisaron:

- Las cinco páginas HTML con navegación interna.
- La identidad visual y el diseño responsive del sitio.
- El catálogo de maquinaria, herramientas, mudanzas y fletes.
- El Hero, las tarjetas informativas y las secciones de Inicio.
- La presentación, línea de tiempo y valores de Nosotros.
- La personalización del Carousel y del Accordion de Bootstrap.
- Los formularios demostrativos de solicitud de presupuesto.
- La arquitectura SCSS modular y su compilación a CSS.
- Mejoras de accesibilidad, SEO básico y carga de imágenes.
- El despliegue del sitio estático en **Netlify**, con el código fuente disponible en **GitHub**.

**Próximas integraciones:** configurar los destinos definitivos de WhatsApp y redes sociales y conectar los formularios de Cotizador y newsletter a un servicio de recepción de datos.

## Autor

**Agustín Tomassini**

Estudiante de Tecnicatura en Informática y formación en Desarrollo Full Stack.

- **GitHub:** [@agxs-tomassini](https://github.com/agxs-tomassini)
- **Repositorio:** [Mr. Trompito – Etapa 2](https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2)

---

Desarrollado por **Agustín Tomassini** como parte de su formación y práctica en desarrollo web.
