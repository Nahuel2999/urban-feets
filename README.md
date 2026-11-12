# URBAN FEETS

Sitio web estático de una tienda de zapatillas, desarrollado como proyecto del curso de **Desarrollo Web** de Coderhouse.

## Descripción

URBAN FEETS reúne en un único catálogo modelos para hombres, mujeres y niños, junto con información sobre ofertas, la tienda y sus medios de contacto.

## Tecnologías

- **HTML5** para la estructura y el contenido.
- **CSS3** para el diseño responsive y los estilos propios.
- **JavaScript de Bootstrap 5.3.3** (bundle oficial por CDN) para los componentes interactivos de Bootstrap; el proyecto no incluye JavaScript propio.
- **Bootstrap 5.3.3** para la navbar, las cards, los badges, los breadcrumbs, el acordeón, las pestañas y los modales.
- **Google Fonts** para las tipografías Poppins y Roboto.
- **Inteligencia artificial generativa** como herramienta de soporte para explorar mejoras, revisar el código y apoyar la documentación. Las propuestas se revisan y adaptan al proyecto.

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
- **Catálogo** (pages/catalogo.html): catálogo unificado con modelos para hombres, mujeres y niños.
- **Ofertas** (pages/ofertas.html): cuatro modelos en oferta, con selector de género.
- **Sobre nosotros** (pages/sobre-nosotros.html): presentación, misión y valores.
- **Contacto** (pages/contacto.html): formulario, datos de contacto y preguntas frecuentes.

## Características

- Navbar adaptable con estado activo por página.
- Breadcrumbs en las páginas internas.
- Tarjetas Bootstrap con alturas y botones alineados.
- Catálogo unificado con 22 modelos únicos; los modelos compartidos permiten elegir género en su tarjeta.
- Modelos exclusivos de mujer y niños integrados en el mismo catálogo.
- Paginación de seis productos por página.
- Selectores de talle del 36 al 46 y modales Bootstrap con información complementaria.
- Badges para identificar las ofertas.
- Preguntas frecuentes en un acordeón Bootstrap.
- Modales con información ampliada de productos.
- Pestañas para organizar la información institucional y las ofertas.
- Navegación directa al catálogo unificado y a la sección de ofertas.
- Aviso visible que aclara que el formulario es una demostración y no envía datos.
- Estilos propios que adaptan los componentes a la paleta de URBAN FEETS.
- Enlaces a Instagram y Facebook.

Los precios, talles y condiciones se utilizan como contenido ficticio de demostración. La paginación muestra hasta seis tarjetas por página.

## Cómo abrir el sitio

No se requiere instalación ni compilación. Abrí index.html en un navegador. Bootstrap y las tipografías requieren conexión a internet.

## Repositorio

[Ver el repositorio en GitHub](https://github.com/Nahuel2999/urban-feets)

## Publicación

La URL de GitHub Pages se agregará cuando el sitio esté publicado.

## Estado

En desarrollo.
