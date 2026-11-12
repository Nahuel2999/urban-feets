# URBAN FEETS

Sitio web estático de una tienda de zapatillas, desarrollado como proyecto del curso de **Desarrollo Web** de Coderhouse.

## Descripción

URBAN FEETS reúne en un único catálogo modelos unisex y para niños, junto con información sobre ofertas, la tienda y sus medios de contacto.

## Tecnologías

- **HTML5** para la estructura y el contenido.
- **CSS3** para el diseño responsive y los estilos propios.
- **Bootstrap 5.3.3** para la navbar, las cards, los badges, los breadcrumbs, el acordeón, las pestañas y los modales.
- **Google Fonts** para las tipografías Poppins y Roboto.
- **ChatGPT (OpenAI)**,** modelo de inteligencia artificial generativa utilizado como herramienta de apoyo para explorar mejoras, revisar el código y organizar la documentación. Las sugerencias se revisan y adaptan al proyecto antes de incorporarse.

Bootstrap y Google Fonts se cargan desde servicios externos mediante CDN, por lo que requieren conexión a internet.

## Estructura del proyecto

~~~text
urban-feets/
├── index.html
├── css/
│   └── styles.css
├── pages/
│   ├── catalogo.html
│   ├── ofertas.html
│   ├── sobre-nosotros.html
│   └── contacto.html
├── assets/
│   └── imágenes y recursos del sitio
~~~

## Páginas

- **Inicio** (index.html): presentación, carrusel, ofertas e información sobre envíos.
- **Catálogo** (pages/catalogo.html): catálogo unificado de modelos con selector de género y opciones para niños.
- **Ofertas** (pages/ofertas.html): cuatro modelos en oferta, con selector de género.
- **Sobre nosotros** (pages/sobre-nosotros.html): presentación, misión y valores.
- **Contacto** (pages/contacto.html): formulario, datos de contacto y preguntas frecuentes.

## Características

- Navbar adaptable con estado activo por página y menú desplegable debajo del encabezado en celular y tablet.
- Breadcrumbs en las páginas internas.
- Tarjetas Bootstrap con alturas y botones alineados.
- Catálogo unificado con 22 modelos; los modelos compartidos permiten elegir género en su tarjeta.
- Opciones de talles del 36 al 46 para adultos y del 20 al 36 para niños.
- Paginación de hasta seis productos por página.
- Modales Bootstrap con información ampliada de los productos.
- Badges para identificar las ofertas.
- Preguntas frecuentes en un acordeón Bootstrap.
- Pestañas para organizar la información institucional y las ofertas.
- Navegación directa al catálogo unificado y a la sección de ofertas.
- Formulario de contacto de demostración, todavía sin conexión a un servicio de envío.
- Estilos propios que adaptan los componentes a la paleta de URBAN FEETS.
- Enlaces a Instagram y Facebook.

Los precios, talles, beneficios y condiciones se utilizan como contenido de demostración.

## Cómo abrir el sitio

No se requiere instalación ni compilación. Abrí index.html en un navegador. Bootstrap y las tipografías requieren conexión a internet.

## Repositorio

[Ver el repositorio en GitHub](https://github.com/Nahuel2999/urban-feets)

## Publicación

El sitio está publicado en GitHub Pages desde la rama `main` y la carpeta raíz.

[Visitar URBAN FEETS](https://nahuel2999.github.io/urban-feets/)

## Estado

Publicado en GitHub Pages.
