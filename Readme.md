# Página Web de JPhone Tech

## Introducción

El proyecto consiste en la creación de una página web para la empresa JPhone Tech. Este documento proporciona una explicación detallada del código HTML utilizado para construir la estructura básica del sitio web, incluyendo la integración de estilos y funcionalidad mediante CSS y Bootstrap.

## Estructura General del Documento HTML

El código HTML del proyecto se organiza de la siguiente manera:

1. **Declaración del Tipo de Documento y Lenguaje:**

   ```html
   <!DOCTYPE html>
   <html lang="en"></html>
   ```

   La primera línea declara el tipo de documento como HTML5. La segunda línea especifica el idioma del contenido como inglés.

2. **Sección `<head>`:**

   ```html
   <head>
     <meta charset="UTF-8" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>Document</title>
     <link rel="stylesheet" href="./style.css" />
     <link
       href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css"
       rel="stylesheet"
       integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH"
       crossorigin="anonymous"
     />
   </head>
   ```

   - **Metaetiquetas:** Definen la codificación de caracteres y la configuración de la vista para dispositivos móviles.
   - **Título de la Página:** Especifica el título del documento.
   - **Enlaces a Estilos:** Incluyen el archivo CSS personalizado (`style.css`) y la biblioteca de Bootstrap.

3. **Sección `<body>`:**
   La sección principal del contenido de la página se encuentra dentro de la etiqueta `<body>` y se organiza en varias partes principales: la barra de navegación, el carrusel de imágenes y el pie de página.

## Barra de Navegación

La barra de navegación permite la navegación entre diferentes secciones del sitio web:

```html
<nav class="navbar navbar-expand-lg bg-black" data-bs-theme="dark">
  <div class="container-fluid nav">
    <img src="./img/logo.png" alt="" class="logo" />
    <a class="navbar-brand text-light" href="#">JPhone Tech</a>
    <button
      class="navbar-toggler"
      type="button"
      data-bs-toggle="collapse"
      data-bs-target="#navbarSupportedContent"
      aria-controls="navbarSupportedContent"
      aria-expanded="false"
      aria-label="Toggle navigation"
    >
      <span class="navbar-toggler-icon"></span>
    </button>
    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav me-auto mb-2 mb-lg-0 menu">
        <li class="nav-item">
          <a class="nav-link" href="#">Inicio</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="./pages/QuienesSomos.html">Quienes somos</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="./pages/productos.html">Productos</a>
        </li>
      </ul>
    </div>
  </div>
</nav>
```

- **Estructura:** Utiliza componentes de Bootstrap para crear una barra de navegación receptiva con enlaces a diferentes páginas.
- **Elementos:** Incluye un logo, el nombre de la empresa, y un menú de navegación con enlaces a "Inicio", "Quienes somos", y "Productos".

## Pie de Página

El pie de página proporciona enlaces a las redes sociales de la empresa:

```html
<footer>
  <div class="container-fluid">
    <div class="row p-5 bg-black text-white">
      <div class="col-xs-12 col-md-6 col-lg-3 footer-logo center">
        <img src="./img/logo.png" alt="" class="logo" />
      </div>
      <div class="col-xs-12 col-md-6 col-lg-3 center">
        <a
          class="text-white text-decoration-none"
          href="https://www.instagram.com/jphone_tech/"
          ><p class="h5">instagram</p></a
        >
      </div>
      <div class="col-xs-12 col-md-6 col-lg-3 center">
        <a
          class="text-white text-decoration-none"
          href="https://wa.me/c/573012267957"
          ><p class="h5">whatsapp</p></a
        >
      </div>
      <div class="col-xs-12 col-md-6 col-lg-3 center">
        <a
          class="text-white text-decoration-none"
          href="https://www.facebook.com/profile.php?id=61553439227489"
          ><p class="h5">facebook</p></a
        >
      </div>
    </div>
  </div>
</footer>
```

- **Enlaces Sociales:** Incluye enlaces a Instagram, WhatsApp y Facebook de la empresa.
- **Diseño Responsivo:** Utiliza el sistema de rejilla de Bootstrap para asegurar que el pie de página sea responsivo y se vea bien en diferentes tamaños de pantalla.

## Integración de Scripts

Finalmente, se incluyen los scripts necesarios para habilitar la funcionalidad de Bootstrap:

```html
<script
  src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
  integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz"
  crossorigin="anonymous"
></script>
```

- **Bootstrap JS:** Se incluye el paquete JavaScript de Bootstrap para habilitar componentes interactivos como el carrusel y la barra de navegación.

#pagina de inicio

## Carrusel de Imágenes

El carrusel proporciona una presentación de diapositivas de imágenes destacadas:

```html
<header>
  <div id="carouselExampleDark" class="carousel carousel-dark slide">
    <div class="carousel-indicators">
      <button
        type="button"
        data-bs-target="#carouselExampleDark"
        data-bs-slide-to="0"
        class="active"
        aria-current="true"
        aria-label="Slide 1"
      ></button>
      <button
        type="button"
        data-bs-target="#carouselExampleDark"
        data-bs-slide-to="1"
        aria-label="Slide 2"
      ></button>
      <button
        type="button"
        data-bs-target="#carouselExampleDark"
        data-bs-slide-to="2"
        aria-label="Slide 3"
      ></button>
    </div>
    <div class="carousel-inner">
      <div class="carousel-item active" data-bs-interval="10000">
        <img src="./img/carousel1.png" class="d-block w-100" alt="..." />
        <div class="carousel-caption d-none d-md-block"></div>
      </div>
      <div class="carousel-item" data-bs-interval="2000">
        <img src="./img/carousel2.png" class="d-block w-100" alt="..." />
        <div class="carousel-caption d-none d-md-block"></div>
      </div>
      <div class="carousel-item">
        <img src="./img/carousel3.png" class="d-block w-100" alt="..." />
        <div class="carousel-caption d-none d-md-block"></div>
      </div>
    </div>
    <button
      class="carousel-control-prev"
      type="button"
      data-bs-target="#carouselExampleDark"
      data-bs-slide="prev"
    >
      <span class="carousel-control-prev-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Previous</span>
    </button>
    <button
      class="carousel-control-next"
      type="button"
      data-bs-target="#carouselExampleDark"
      data-bs-slide="next"
    >
      <span class="carousel-control-next-icon" aria-hidden="true"></span>
      <span class="visually-hidden">Next</span>
    </button>
  </div>
</header>
```

- **Componentes de Bootstrap:** Se utiliza el componente de carrusel de Bootstrap para crear un pase de diapositivas automático.
- **Imágenes y Controles:** Cada elemento del carrusel incluye una imagen y controles para navegar entre las diapositivas.

# Pagina Quienes somos

# Explicación del Contenido: Sección "Quiénes Somos"

La sección proporciona información sobre la empresa JPhone_Tech y su enfoque en tecnología móvil, específicamente en productos Apple. Aquí está un desglose de cada elemento:

## Contenedor de la Sección

```html
<section class="w-50 mx-auto text-center"></section>
```

- **Clases CSS:** La sección se coloca en el centro de la página con un ancho del 50% del contenedor principal (`w-50`) y se centra horizontalmente (`mx-auto`). El texto dentro de la sección se alinea al centro (`text-center`).

## Título Principal

```html
<h1 class="title">Quienes somos</h1>
```

- **Elemento `<h1>`:** Este elemento representa el título principal de la sección, que es "Quienes somos". Se le asigna una clase CSS personalizada llamada "title".

## Párrafos de Texto

```html
<p>...</p>
```

- **Elemento `<p>`:** Se utilizan varios elementos de párrafo para proporcionar información sobre la empresa JPhone_Tech.
- **Contenido:** Los párrafos describen la dedicación de la empresa a ofrecer productos de tecnología móvil, especialmente de Apple, su amplia gama de productos y accesorios, así como el compromiso con la calidad, autenticidad y servicio al cliente.

## Imagen de la Marca

```html
<img src="../img/marca.png" alt="" class="marca" />
```

- **Elemento `<img>`:** Muestra una imagen de la marca JPhone_Tech.
- **Atributos:** El atributo `src` especifica la ruta de la imagen, mientras que el atributo `alt` proporciona un texto alternativo para accesibilidad.
- **Clase CSS:** Se le asigna la clase "marca", que puede ser utilizada para aplicar estilos específicos a esta imagen.

Esta sección proporciona una descripción detallada de la empresa JPhone_Tech, su enfoque en productos Apple, su compromiso con la calidad y el servicio al cliente, y alienta a los usuarios a explorar más sobre la empresa a través de sus canales en línea y locales físicos. La imagen de la marca ayuda a reforzar la identidad visual de la empresa dentro del contenido de la página.

# Pagina Productos

# Explicación del Contenido: Sección de Productos

La sección muestra una selección de productos disponibles en la tienda JPhone_Tech. Aquí está un desglose de cada elemento:

## Contenedor de la Sección

```html
<section class="mx-auto text-center ancho">
```

- **Clases CSS:** La sección se coloca en el centro de la página y se le asigna una clase llamada "ancho" para establecer su ancho máximo. Además, se centra horizontalmente el contenido de la sección.

## Filas de Productos

```html
<div class="row row-cols-1 row-cols-md-3 g-4 espacio">
```

- **Clases CSS:** Se utiliza una fila con clases de Bootstrap para organizar los productos en una cuadrícula de tres columnas en dispositivos de tamaño medio (`md`) y una columna en dispositivos pequeños (`col-1`). La clase `g-4` agrega un espacio entre las columnas, y la clase `espacio` puede aplicar estilos adicionales si es necesario.

## Tarjetas de Productos

```html
<div class="col">
    <div class="card h-100">
        <img src="../img/producto4.jpeg" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title">Airpods Max Negro</h5>
            <p class="card-text">Los AirPods Max ofrecen audio excepcional con cancelación de ruido y hasta 20 horas de batería. Disfruta de diseño elegante, comodidad superior y conectividad perfecta con tus dispositivos Apple.</p>
        </div>
        <div class="card-footer">
            <small class="text-body-secondary">COP $110.000</small>
        </div>
    </div>
</div>
```

- **Clases CSS:** Cada columna contiene una tarjeta de producto.
- **Imagen:** Se muestra una imagen del producto con la clase `card-img-top`.
- **Título y Descripción:** Se muestra el nombre del producto y una breve descripción del mismo.
- **Precio:** Se muestra el precio del producto dentro del pie de página de la tarjeta.

Esta sección presenta una variedad de productos disponibles en la tienda JPhone_Tech, cada uno con su propia imagen, descripción y precio. Las tarjetas de productos están diseñadas de manera uniforme para una presentación coherente y atractiva. La organización en una cuadrícula facilita la navegación y la comparación de productos para los visitantes del sitio web.

## Conclusión

Este proyecto de página web para JPhone Tech utiliza HTML5 y Bootstrap 5 para crear una estructura moderna y responsiva. La página incluye una barra de navegación intuitiva, un carrusel de imágenes atractivo y un pie de página con enlaces a las redes sociales de la empresa. Este enfoque asegura que la página sea fácil de usar y visualmente atractiva en diferentes dispositivos y tamaños de pantalla.
