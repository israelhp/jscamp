# Modulo 2

## Que es HTML

👨‍💻 HTML: Los Primeros Pasos para Crear tu Web
Vamos a adentrarnos en el mundo de HTML, la columna vertebral de cualquier página web. Entender HTML es fundamental porque es el lenguaje que utilizamos para estructurar el contenido que vemos en internet.

🤔 ¿Qué es HTML?
HTML, o HyperText Markup Language, no es un lenguaje de programación como JavaScript. Es un lenguaje de marcado que te permite organizar y describir los diferentes elementos de una página web, como textos, imágenes, enlaces, listas y tablas. Piensa en él como el esqueleto de tu sitio web.

🧱 Estructura Básica de un Documento HTML
Todo documento HTML sigue una estructura básica. Aquí te explico los dos primeros elementos principales:

- `<!DOCTYPE html>`: Esta declaración le dice al navegador que estás usando la versión más reciente de HTML (HTML5). Siempre va al principio de tu documento.
- `<html lang="es">`: Es el elemento raíz que engloba todo el contenido de tu página. El atributo lang="es" indica que el idioma principal del contenido es el español.
  ¡Ten en cuenta que la declaración <!DOCTYPE html> no es una etiqueta HTML! Es una declaración que le dice al navegador que estás usando la versión más reciente de HTML (HTML5).

📝 Nuestro Primer Documento HTML
Vamos a crear un archivo index.html con esta estructura para nuestro proyecto DevJobs. Aquí te dejo un ejemplo de cómo se vería una página básica. ¡Intenta replicarlo!

```html
<!DOCTYPE html>
<html lang="es"></html>
```

Ahora vamos a ver más elementos para estructurar nuestra página.

¿Cómo son los elementos en HTML?
Los elementos en HTML son las etiquetas que se utilizan para estructurar el contenido de la página. Se componen, normalmente, de una etiqueta de apertura y una etiqueta de cierre. Dentro de ellas, se encuentra el contenido del elemento.

```html
<p>Este es un párrafo</p>
```

En este ejemplo, la etiqueta <p> es el elemento que se utiliza para crear un párrafo.

Además los elementos pueden tener atributos. Los atributos son información adicional que se puede añadir a los elementos.

```html
<button type="submit">Este es un botón</button>
```

En este ejemplo, el atributo type es el atributo que se utiliza para crear un botón del tipo “submit”. A lo largo del curso iremos conociendo nuevos y más atributos que nos permitirán crear elementos más complejos.

De hecho, si te fijas, ya hemos visto un atributo en el ejemplo de la estructura básica de un documento HTML.

```html
<html lang="es"></html>
```


## La estructura basica 

En este ejemplo, el atributo lang es el atributo que se utiliza para indicar el idioma del documento.

La Estructura Básica de HTML
Al finalizar esta clase serás capaz de:

✅ Entender la estructura fundamental de un documento HTML
✅ Conocer la función de las etiquetas <head> y <body>
✅ Implementar metadatos esenciales para tu página web
✅ Crear una base sólida para tu primera página web

🧠 La Cabeza del Documento: <head>
La etiqueta <head> es como el cerebro de tu documento HTML. Contiene información crucial que no es visible para el usuario, pero que es fundamental para el funcionamiento de la página.

💡 Dato importante: Si pones texto directamente en <head>, no aparecerá en la página. Su función es describir el documento, no mostrarlo.

📋 Elementos esenciales del <head>
1. Codificación de caracteres
```html
<meta charset="UTF-8">
```

¿Para qué sirve?

* Permite mostrar correctamente tildes, eñes, símbolos y emojis
* Sin esto verías caracteres extraños como Ã± en lugar de ñ

2. Viewport para dispositivos móviles
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
¿Para qué sirve?

* Hace que tu página se vea bien en móviles y tablets
* Es fundamental para el diseño responsive
* Le dice al navegador cómo escalar la página en diferentes pantallas

3. Título de la página
```html
<title>DevJobs - Inicio</title>
```

¿Para qué sirve?

* Aparece en la pestaña del navegador
* Se muestra en los resultados de Google
* Debe ser descriptivo y único para cada página

4. Descripción para buscadores
```html
<meta name="description" content="Encuentra las mejores ofertas de trabajo para desarrolladores en DevJobs.">
```
¿Para qué sirve?

* SEO: Google la usa en los resultados de búsqueda
* Aparece como el texto descriptivo debajo del título
* Debe ser atractiva y resumir el contenido de la página

🔍 Ejemplo práctico: Si buscas “midudev” en Google, la descripción que aparece debajo del título proviene de esta metaetiqueta.

👁️ El Cuerpo del Documento: <body>
La etiqueta `<body>` es donde vive todo el contenido visible de tu página web. Es lo que los usuarios realmente ven e interactúan.

🎨 ¿Qué va dentro de <body>?

| Tipo de contenido| Ejemplos |
|---|---|
| Texto | Parrafos,titulos,listas|
|Multimedia	| Imágenes, videos, audio|
|Interactivos	|Formularios, botones, enlaces|
|Estructura	| Navegación, secciones, artículos|

🏗️ Construcción del marcado
En <body> es donde construiremos toda la estructura de DevJobs:

* Header con navegación
* Secciones de contenido
* Formularios de búsqueda
* Listado de trabajos
* Footer

📝 Estructura completa básica
```html
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>DevJobs - Inicio</title>
    <meta name="description" content="Encuentra las mejores ofertas de trabajo para desarrolladores en DevJobs.">
</head>
<body>
    <!-- Aquí va todo el contenido visible -->
    <h1>¡Hola mundo!</h1>
    <p>Este es mi primer documento HTML.</p>
</body>
</html>
```


## La etiqueta body y mas 

El Cuerpo del Documento: `<body>`

Después de la etiqueta `<head>`, viene la etiqueta `<body>`. Este es el cuerpo de tu documento HTML y es donde va todo el contenido visible de tu página web.

Contenido visible: Textos, imágenes, videos, formularios, enlaces, botones, tablas… absolutamente todo lo que el usuario ve e interactúa directamente se coloca dentro de `<body>`.

Construcción del marcado: Es en `<body>` donde empezaremos a construir todo el marcado de DevJobs, utilizando las diferentes etiquetas HTML para dar forma a nuestro contenido.

Construyendo el contenido de DevJobs
Vamos a empezar a construir el header de DevJobs, donde está el logo y la navegación. Vamos a ir añadiendo poco a poco los elementos que necesitamos, describiendo el contenido usando diferentes etiquetas HTML.

```html 
<body>
  <header>
    <h2>DevJobs</h2>

    <nav>
      <a href="#">Inicio</a>
      <a href="#">Empleos</a>
    </nav>

    <div>
      <a href="#">Publicar un empleo</a>
      <a href="#">Iniciar sesión</a>
    </div>
  </header>
</body>
```

Ahora mismo no nos preocupamos sobre cómo se ve, simplemente estamos describiendo el contenido de la página usando diferentes etiquetas HTML.

Elementos HTML nuevos explicados:

`<header>`
Elemento semántico (tiene significado)
Le dice al navegador: “esto es el encabezado”
Puede haber varios headers en una página (uno principal y otros en secciones)
NO confundir con `<head>` (que es metadatos, el que vimos antes)

`<h2>`
Heading 2 (Encabezado de nivel 2)
Los headings van del `<h1>` al `<h6>` (como los títulos en Word)
Jerarquía: h1 > h2 > h3 > h4 > h5 > h6
¿Por qué h2 y no h1? Reservamos h1 para el título principal del contenido

`<nav>`
Navigation (navegación)
Elemento semántico para menús de navegación
Google y lectores de pantalla lo reconocen como navegación principal

`<a href="...">`
* Anchor (ancla) - crea un enlace
* href = hypertext reference (referencia de hipertexto)
* Tipos de valores para href:
    * href="/" = página principal (home)
    * href="/empleos" = ruta relativa
    * href="https://google.com" = URL completa
    * href="#" = placeholder (no lleva a ningún lado, temporal)
    * href="#seccion" = ancla a una sección de la misma página
* El elemento <a> es uno de los más importantes en HTML, porque nos permite crear enlaces a otras páginas o a secciones de la misma página. Es la base de la navegación en la web.


`<div>`

* Division (división)
* Es un contenedor genérico SIN significado semántico
* Se usa para agrupar elementos cuando no hay un elemento semántico apropiado
* Es como una caja invisible para organizar
* El elemento <div> es un elemento muy popular, ya que nos permite agrupar elementos… sólo hay que tener cuidado de no usarlo cuando haya un mejor elemento semántico para el contenido que estamos creando.