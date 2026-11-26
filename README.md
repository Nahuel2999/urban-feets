
# URBAN FEETS

Sitio web estático de una tienda de zapatillas, desarrollado como proyecto del curso de **Desarrollo Web** de Coderhouse.

## Descripción

URBAN FEETS reúne en un único catálogo modelos unisex y para niños, junto con información sobre ofertas, la tienda y sus medios de contacto.

El proyecto cuenta con un diseño responsive y una arquitectura de estilos modular basada en SCSS, orientada a facilitar la organización, reutilización y mantenimiento del código.

## Tecnologías

- **HTML5** para la estructura y el contenido.
- **CSS3** para el diseño responsive y la aplicación de los estilos compilados.
- **Sass (SCSS)** para la organización modular de los estilos mediante partials, variables, mixins, nesting y el operador `&`.
- **Bootstrap 5.3.3** para la navbar, las cards, los badges, los breadcrumbs, el acordeón, las pestañas y los modales.
- **JavaScript** para las funcionalidades interactivas del sitio.
- **Google Fonts** para las tipografías Poppins y Roboto.
- **Node.js y npm** para instalar la versión de Sass del proyecto y ejecutar los scripts de compilación.
- **Git** para el control de versiones y la gestión de ramas.
- **GitHub** para el almacenamiento y seguimiento del proyecto.
- **GitHub Pages** para la publicación del sitio web.
- **ChatGPT (OpenAI)** como herramienta de apoyo para explorar mejoras, revisar el código y organizar la documentación. Las sugerencias se revisan y adaptan al proyecto antes de incorporarse.

Bootstrap y Google Fonts se cargan desde servicios externos mediante CDN, por lo que requieren conexión a internet.

## Estructura del proyecto

~~~text
urban-feets/
├── index.html
├── README.md
├── .gitignore
├── package.json
├── package-lock.json
├── assets/
│   └── imágenes y recursos del sitio
├── css/
│   ├── styles.css
│   └── styles.css.map
├── pages/
│   ├── catalogo.html
│   ├── ofertas.html
│   ├── sobre-nosotros.html
│   └── contacto.html
└── scss/
    ├── main.scss
    ├── utilities/
    │   ├── _variables.scss
    │   └── _mixins.scss
    ├── base/
    │   ├── _base.scss
    │   └── _tipografia.scss
    ├── layout/
    │   ├── _header.scss
    │   ├── _nav.scss
    │   ├── _content.scss
    │   └── _footer.scss
    └── components/
        ├── _buttons.scss
        ├── _cards.scss
        ├── _forms.scss
        ├── _carousel.scss
        ├── _accordion.scss
        ├── _tabs.scss
        └── _pagination.scss
~~~

## Arquitectura SCSS

Los estilos propios del proyecto se encuentran organizados en una estructura modular de archivos SCSS.

### Utilities

Contiene los recursos reutilizables del sistema de estilos.

- `_variables.scss`: colores, espaciados, bordes, sombras, transiciones y puntos de quiebre responsivos.
- `_mixins.scss`: mixins con parámetros para el borde y el relleno de botones y enlaces del menú, el ajuste de imágenes y los estados de foco.

### Base

Contiene los estilos generales del sitio.

- `_base.scss`: estilos globales y propiedades generales.
- `_tipografia.scss`: configuración tipográfica.

### Layout

Contiene los estilos relacionados con la estructura y distribución del sitio.

- `_header.scss`: encabezado.
- `_nav.scss`: navegación y personalización de la navbar.
- `_content.scss`: distribución del contenido principal.
- `_footer.scss`: pie de página.

### Components

Contiene los estilos de los elementos reutilizables del sitio y la personalización de componentes de Bootstrap.

- `_buttons.scss`: botones.
- `_cards.scss`: tarjetas de productos.
- `_forms.scss`: formularios.
- `_carousel.scss`: carruseles.
- `_accordion.scss`: acordeones.
- `_tabs.scss`: pestañas.
- `_pagination.scss`: paginación.

### Archivo maestro

El archivo `main.scss` constituye el único punto de entrada para la compilación de los estilos.

Los `@use` se agrupan al comienzo en el orden `utilities → base → layout → components`. A continuación, los `@include` incorporan los estilos en el orden de la cascada.

El archivo `css/styles.css` es generado automáticamente mediante Sass y no debe editarse de forma manual.

## Páginas

- **Inicio** (`index.html`): presentación, carrusel, ofertas e información sobre envíos.
- **Catálogo** (`pages/catalogo.html`): catálogo unificado de modelos con selector de género y opciones para niños.
- **Ofertas** (`pages/ofertas.html`): cuatro modelos en oferta, con selector de género.
- **Sobre nosotros** (`pages/sobre-nosotros.html`): presentación, misión y valores.
- **Contacto** (`pages/contacto.html`): formulario, datos de contacto y preguntas frecuentes.

## Características

- Diseño responsive adaptable a celulares, tablets y computadoras.
- Navbar adaptable con estado activo por página y menú desplegable.
- Breadcrumbs en las páginas internas.
- Tarjetas Bootstrap con alturas y botones alineados.
- Catálogo unificado con 22 modelos.
- Selectores de género y talle.
- Opciones de talles del 36 al 46 para adultos y del 20 al 35 para niños.
- Paginación de hasta seis productos por página.
- Modales Bootstrap con información ampliada de los productos.
- Badges para identificar las ofertas.
- Preguntas frecuentes en un acordeón Bootstrap.
- Pestañas para organizar la información institucional y las ofertas.
- Navegación directa al catálogo unificado y a la sección de ofertas.
- Formulario de contacto de demostración, todavía sin conexión a un servicio de envío.
- Personalización de componentes Bootstrap mediante SCSS.
- Arquitectura modular de estilos basada en partials.
- Reutilización de valores mediante variables Sass.
- Reutilización de estilos mediante mixins.
- Organización de selectores mediante nesting y el operador `&`.
- Enlaces a Instagram y Facebook.

Los precios, talles, beneficios y condiciones se utilizan como contenido de demostración.

## Cómo abrir el sitio

Para visualizar el sitio no se requiere instalación ni compilación adicional, ya que el repositorio incluye la hoja de estilos compilada.

Clonar el repositorio:

~~~bash
git clone https://github.com/Nahuel2999/urban-feets.git
~~~

Ingresar al directorio del proyecto:

~~~bash
cd urban-feets
~~~

Abrir el archivo `index.html` en un navegador.

Bootstrap y las tipografías requieren conexión a internet.

## Compilación de SCSS

Para modificar los estilos, necesitás Node.js 20.19.0 o superior y npm. Ejecutá los comandos desde la raíz del proyecto, donde está `package.json`.

### Instalación de Sass

~~~bash
npm ci
~~~

Sass se instala como dependencia de desarrollo según las versiones registradas en `package-lock.json`. Git ignora la carpeta `node_modules/`.

### Compilación manual

Desde el directorio raíz del proyecto:

~~~bash
npm run build:css
~~~

El comando compila `scss/main.scss` y genera `css/styles.css` y `css/styles.css.map`.

### Compilación automática

Para detectar modificaciones en los archivos SCSS y actualizar automáticamente la hoja de estilos:

~~~bash
npm run watch:css
~~~

Para detener la compilación automática, utilizar `Ctrl + C` en la terminal.

Todas las modificaciones relacionadas con los estilos deben realizarse en los archivos SCSS.

## Control de versiones

El proyecto utiliza Git como sistema de control de versiones y GitHub como repositorio remoto.

### Ramas

- `main`: rama principal del proyecto.
- `demo-branch`: rama de desarrollo de funcionalidades y componentes interactivos.
- `scss-branch`: rama de desarrollo de la arquitectura SCSS y refactorización de estilos.

Las modificaciones desarrolladas en las ramas secundarias se encuentran integradas en la rama principal.

El historial de commits conserva las distintas etapas de desarrollo y refactorización del proyecto.

## Repositorio

[Ver el repositorio en GitHub](https://github.com/Nahuel2999/urban-feets)

## Publicación

El sitio está publicado en GitHub Pages desde la rama `main` y la carpeta raíz.

[Visitar URBAN FEETS](https://nahuel2999.github.io/urban-feets/)

## Estado

- Sitio web funcional.
- Diseño responsive implementado.
- Componentes Bootstrap personalizados.
- Arquitectura SCSS modular implementada.
- Refactorización de estilos completada.
- Ramas de desarrollo integradas en `main`.
- Publicado en GitHub Pages.

Proyecto académico desarrollado en el marco del curso de Desarrollo Web de Coderhouse.
