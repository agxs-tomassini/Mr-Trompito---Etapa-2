Mr. Trompito | Maquinaria, Mudanzas y Fletes
Sitio web de Mr. Trompito, un emprendimiento dedicado al alquiler de maquinaria y herramientas para la construcción, así como a los servicios de mudanzas, fletes y traslado de materiales en Buenos Aires, Argentina.

El proyecto fue desarrollado como parte de mi formación en Desarrollo Web, con un enfoque en diseño responsive, organización modular de estilos, experiencia de usuario y mantenimiento del código.
Sitio web publicado
- Sitio en línea (Netlify): PEGAR_AQUI_LA_URL_DE_NETLIFY
- Repositorio de GitHub: Mr-Trompito---Etapa-2
La versión pública del sitio se aloja en Netlify. El código fuente se administra en GitHub, utilizando la rama main para el despliegue del sitio.

Tecnologías utilizadas
- HTML5: estructura semántica y formularios.
- CSS3: estilos personalizados, animaciones y estados de interacción.
- Sass (SCSS): variables, mixins, anidamiento, @extend y arquitectura modular con @use.
- Bootstrap 5.3.3: sistema de grillas, navbar responsive, carrusel, acordeón y componentes de formularios.
- Bootstrap Icons: iconografía de servicios, navegación y acciones.
- Animate.css: animaciones de entrada en títulos.
- Flexbox y CSS Grid: distribución adaptable de tarjetas, secciones y paneles.
- Google Fonts: Barlow Condensed, Noto Sans y Petit Formal Script.
- Git y GitHub: control de versiones y repositorio del proyecto.
- Netlify: alojamiento y publicación del sitio estático.

Páginas del sitio
Página	Archivo	Contenido
Inicio	index.html	Presentación del emprendimiento, servicios destacados, tarjetas informativas, galería y acceso a otras secciones.
Servicios	pages/servicios.html	Catálogo de maquinaria, herramientas, mudanzas y fletes, con enlaces al cotizador.
Nosotros	pages/nosotros.html	Historia del emprendimiento, línea de tiempo y valores de trabajo.
Preguntas frecuentes	pages/faq.html	Preguntas y respuestas organizadas mediante un acordeón de Bootstrap.
Cotizador	pages/cotizador.html	Formularios para consultas sobre alquiler de maquinaria y mudanzas/fletes.


Funcionalidades e interfaz
- Navegación responsive: menú horizontal en escritorio y menú colapsable en pantallas más pequeñas.
- Inicio: Hero con contenido destacado y dos imágenes, tarjetas de confianza, servicios principales y enlace a la historia del emprendimiento.
- Catálogo: tarjetas organizadas con CSS Grid en una, dos o tres columnas según el dispositivo; las imágenes no disponibles se indican con un marcador visual.
- Galería: carrusel de Bootstrap con cinco imágenes y navegación manual mediante flechas e indicadores.
- Nosotros: presentación visual, línea de tiempo de tres etapas y panel con valores de puntualidad, seriedad y cuidado.
- FAQ: acordeón interactivo de Bootstrap para consultar las preguntas frecuentes.
- Cotizador: dos formularios diferenciados, con etiquetas asociadas a los campos y validaciones nativas de HTML.
- Footer: información del emprendimiento, enlaces a redes sociales y formulario de newsletter.
Diseño responsive e identidad visual
El sitio se rediseñó con una identidad visual consistente en sus cinco páginas.

Paleta de colores
Uso	Color
Principal, azul marino	#0b1f3b
Acento, azul	#2563eb
Secundario, celeste	#60a5fa
Superficies	#dbeafe
Fondo general	#f2f7fc
Detalles decorativos, naranja	#e75319


Tipografías
- Barlow Condensed: títulos y enlaces destacados.
- Noto Sans: textos y descripciones.
- Petit Formal Script: palabras y fragmentos decorativos.
Los diseños se adaptan mediante la grilla de Bootstrap y breakpoints definidos en SCSS. Se emplean efectos hover, sombras, detalles decorativos y estados de foco para mantener una interfaz coherente.
Accesibilidad y rendimiento
Durante el desarrollo se incorporaron mejoras de estructura, interacción y carga:
- Etiquetas semánticas y jerarquía de encabezados en las cinco páginas.
- Textos alternativos para las fotografías y etiquetas asociadas a los campos de formularios.
- Atributos ARIA en componentes interactivos como el menú y el acordeón.
- Estados :focus-visible para facilitar la navegación mediante teclado.
- Reglas prefers-reduced-motion para reducir animaciones personalizadas.
- Navegación manual del carrusel para evitar el avance automático de contenido.
- Ajustes de imágenes y prioridad de carga para la fotografía principal del Hero.
- Títulos y metadescripciones específicos para cada página.
Estructura del proyecto
Mr-Trompito---Etapa-2/
├── index.html
├── pages/
│   ├── servicios.html
│   ├── nosotros.html
│   ├── faq.html
│   └── cotizador.html
├── assets/
├── scss/
│   ├── main.scss
│   ├── utilities/
│   │   ├── _variables.scss
│   │   └── _mixins.scss
│   ├── base/
│   │   ├── _base.scss
│   │   └── _tipografia.scss
│   ├── layout/
│   │   ├── _header.scss
│   │   ├── _nav.scss
│   │   └── _footer.scss
│   └── components/
│       ├── _buttons.scss
│       ├── _cards.scss
│       ├── _forms.scss
│       ├── _carousel.scss
│       ├── _accordion.scss
│       ├── _home.scss
│       └── _nosotros.scss
├── styles/
│   └── main.css
├── package.json
└── README.md
scss/main.scss importa los módulos mediante @use. El CSS que utilizan las páginas HTML se genera en styles/main.css.
Ejecutar el proyecto localmente
1. Clonar el repositorio
git clone https://github.com/agxs-tomassini/Mr-Trompito---Etapa-2.git
cd Mr-Trompito---Etapa-2
2. Instalar las dependencias
npm install
3. Compilar los estilos SCSS

Compilación única:
npx sass scss/main.scss styles/main.css --no-source-map
Compilación automática durante el desarrollo:
npx sass --watch scss/main.scss:styles/main.css
4. Abrir el sitio

Abrir index.html en el navegador o utilizar la extensión Live Server de Visual Studio Code.
El archivo styles/main.css se genera desde Sass. Los cambios de estilo deben realizarse en los archivos de scss/, no directamente en el CSS compilado.

Despliegue en Netlify
Mr. Trompito es un sitio frontend estático, por lo que no requiere un servidor de aplicaciones para mostrar sus páginas. Netlify distribuye los archivos HTML, CSS e imágenes de la versión publicada.

La configuración prevista para la publicación del repositorio es:
Parámetro	Valor
Repositorio	agxs-tomassini/Mr-Trompito---Etapa-2
Rama de producción	main
Directorio de publicación	Raíz del repositorio (.)
Comando de compilación	No requerido si styles/main.css está incluido en el repositorio


Con el repositorio vinculado a Netlify, las nuevas versiones pueden publicarse mediante los cambios enviados a main.
Alcance de la versión publicada
La versión alojada en Netlify presenta la interfaz y la navegación de las cinco páginas, incluidos los componentes interactivos de Bootstrap.

Funcionalidades pendientes de integración:
- Los formularios de Cotizador y newsletter son demostrativos: actualmente usan action="#" y no envían datos a un servicio de procesamiento ni generan cotizaciones automáticas.
- Los enlaces de WhatsApp y redes sociales son provisionales y se reemplazarán por los canales definitivos del emprendimiento.
Estas integraciones no forman parte del frontend estático implementado en esta versión.
Autor
Agustín Tomassini
Estudiante de Tecnicatura en Informática y en formación en Desarrollo Full Stack.
- Perfil de GitHub
- Código fuente de Mr. Trompito
Proyecto realizado como parte de mi formación en desarrollo web.