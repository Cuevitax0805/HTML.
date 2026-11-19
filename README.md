# HTML — ELEMENTOS Y ESTRUCTURAS BÁSICAS

Repositorio de recopilación, documentación y aprendizaje de los elementos fundamentales de HTML (HyperText Markup Language).

Este repositorio contiene una guía de referencia sobre la estructura de los documentos HTML, sus etiquetas, atributos, elementos semánticos, formularios, tablas y recursos multimedia.

---

## 📑 ÍNDICE

1. [Introducción a HTML](#1-introducción-a-html)
2. [Estructura básica de un documento](#2-estructura-básica-de-un-documento)
3. [Elementos de metadatos](#3-elementos-de-metadatos)
4. [Etiquetas y elementos HTML](#4-etiquetas-y-elementos-html)
5. [Atributos HTML](#5-atributos-html)
6. [Elementos de texto](#6-elementos-de-texto)
7. [Encabezados y secciones](#7-encabezados-y-secciones)
8. [Elementos semánticos](#8-elementos-semánticos)
9. [Enlaces y rutas](#9-enlaces-y-rutas)
10. [Listas](#10-listas)
11. [Tablas](#11-tablas)
12. [Formularios](#12-formularios)
13. [Elementos multimedia](#13-elementos-multimedia)
14. [Contenido incrustado](#14-contenido-incrustado)
15. [Elementos de agrupación](#15-elementos-de-agrupación)
16. [Caracteres especiales y entidades HTML](#16-caracteres-especiales-y-entidades-html)
17. [Comentarios en HTML](#17-comentarios-en-html)
18. [Integración con CSS y JavaScript](#18-integración-con-css-y-javascript)
19. [Accesibilidad y buenas prácticas](#19-accesibilidad-y-buenas-prácticas)
20. [Estructura de un proyecto HTML](#20-estructura-de-un-proyecto-html)

---

## 1. INTRODUCCIÓN A HTML

HTML (HyperText Markup Language) es un lenguaje de marcado utilizado para estructurar y organizar el contenido de las páginas web.

Permite definir elementos como títulos, párrafos, imágenes, enlaces, tablas, formularios y contenido multimedia.

HTML no es un lenguaje de programación: es un lenguaje de marcado que utiliza etiquetas para indicar la estructura y el significado del contenido.

### Características principales

- Define la estructura de una página web.
- Organiza el contenido mediante etiquetas.
- Permite incorporar imágenes, audio y vídeo.
- Facilita la navegación mediante enlaces.
- Se integra con CSS para definir la presentación visual.
- Se integra con JavaScript para incorporar interactividad.

---

## 2. ESTRUCTURA BÁSICA DE UN DOCUMENTO

Todo documento HTML debe contar con una estructura básica que permita al navegador interpretar correctamente su contenido.

### Ejemplo:

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Mi primera página</title>
</head>

<body>

    <h1>Hola, mundo</h1>
    <p>Mi primera página web utilizando HTML.</p>

</body>
</html>
```

### Elementos de inicio

| Etiqueta | Función |
|---|---|
| `<!DOCTYPE html>` | Declara que el documento utiliza HTML5. |
| `<html>` | Elemento raíz del documento HTML. |
| `<head>` | Contiene los metadatos y referencias a recursos. |
| `<body>` | Contiene el contenido visible de la página. |

### Explicación de la estructura

- `<!DOCTYPE html>`: indica al navegador que interprete el documento utilizando el estándar HTML.
- `<html>`: contiene todos los elementos del documento.
- `<head>`: almacena información de configuración y metadatos.
- `<body>`: contiene los elementos que forman el contenido de la página.

---

## 3. ELEMENTOS DE METADATOS

Los metadatos proporcionan información sobre el documento HTML. Generalmente se encuentran dentro de la etiqueta `<head>` y no forman parte del contenido visible de la página.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<head>` | Contiene los metadatos del documento. |
| `<title>` | Define el título de la página en la pestaña del navegador. |
| `<meta>` | Proporciona información sobre el documento. |
| `<link>` | Establece relaciones con recursos externos. |
| `<style>` | Permite incorporar reglas CSS dentro del documento. |
| `<script>` | Permite incorporar o enlazar código JavaScript. |
| `<base>` | Define una URL base para las rutas relativas del documento. |

### Ejemplo:

```html
<head>

    <meta charset="UTF-8">

    <meta name="description" content="Página de aprendizaje HTML">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Aprendiendo HTML</title>

    <link rel="stylesheet" href="estilos.css">

    <style>
        body {
            font-family: Arial, sans-serif;
        }
    </style>

    <script src="script.js" defer></script>

</head>
```

### Conceptos importantes

- `charset`: establece la codificación de caracteres.
- `description`: proporciona una descripción del contenido de la página.
- `viewport`: permite adaptar la presentación a las dimensiones de los dispositivos.
- `href`: indica la ubicación del recurso enlazado.
- `defer`: permite ejecutar un script externo después de analizar el documento HTML.

---

## 4. ETIQUETAS Y ELEMENTOS HTML

HTML utiliza etiquetas para definir los diferentes elementos que componen una página web.

### Elementos con apertura y cierre

La mayoría de los elementos HTML utilizan una etiqueta de apertura y otra de cierre.

```html
<p>Este es un párrafo.</p>
```

- `<p>`: etiqueta de apertura.
- `Este es un párrafo.`: contenido.
- `</p>`: etiqueta de cierre.

### Elementos vacíos

Algunos elementos HTML no tienen contenido interno ni necesitan etiqueta de cierre.

```html
<img src="imagen.jpg" alt="Descripción de la imagen">

<br>

<hr>

<input type="text">
```

Ejemplos:

- `<img>`: incorpora una imagen.
- `<br>`: introduce un salto de línea.
- `<hr>`: representa una separación temática.
- `<input>`: crea un control de entrada.

---

## 5. ATRIBUTOS HTML

Los atributos proporcionan información adicional sobre los elementos HTML y permiten modificar su comportamiento o configuración.

Se escriben dentro de la etiqueta de apertura.

### Ejemplo:

```html
<a href="https://www.google.com" target="_blank">
    Visitar Google
</a>
```

En este ejemplo:

- `href`: indica la dirección del enlace.
- `target`: determina dónde se abrirá el recurso.
- `_blank`: abre el enlace en una nueva pestaña o contexto.

### Atributos comunes

| Atributo | Función |
|---|---|
| `id` | Identifica de manera única un elemento dentro del documento. |
| `class` | Agrupa elementos para aplicar estilos o seleccionarlos mediante JavaScript. |
| `style` | Permite aplicar estilos CSS directamente. |
| `title` | Proporciona información adicional sobre un elemento. |
| `src` | Define la ubicación de un recurso externo. |
| `href` | Define la dirección de un enlace. |
| `alt` | Proporciona un texto alternativo para las imágenes. |
| `width` | Define el ancho de un elemento compatible. |
| `height` | Define la altura de un elemento compatible. |
| `name` | Identifica un control o dato enviado por un formulario. |
| `value` | Define el valor de un control. |
| `disabled` | Deshabilita un control. |
| `required` | Indica que un campo es obligatorio. |
| `placeholder` | Muestra una indicación dentro de un campo. |

### Atributos globales

Son atributos que pueden utilizarse en la mayoría de los elementos HTML.

```html
<p id="parrafo-principal" class="texto" title="Información adicional">
    Ejemplo de atributos globales.
</p>
```

---

## 6. ELEMENTOS DE TEXTO

Permiten organizar, representar y dar significado al contenido textual de una página.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<h1>` a `<h6>` | Definen encabezados de diferentes niveles. |
| `<p>` | Define un párrafo. |
| `<strong>` | Indica que el contenido tiene gran importancia. |
| `<em>` | Añade énfasis al contenido. |
| `<b>` | Llama la atención sobre un texto sin añadir importancia semántica. |
| `<i>` | Representa texto en una voz o estilo diferente. |
| `<u>` | Representa una anotación o texto subrayado. |
| `<small>` | Representa contenido secundario o de menor importancia. |
| `<mark>` | Resalta un fragmento de texto. |
| `<del>` | Representa contenido eliminado. |
| `<ins>` | Representa contenido insertado. |
| `<sub>` | Define un subíndice. |
| `<sup>` | Define un superíndice. |
| `<code>` | Representa fragmentos de código. |
| `<pre>` | Conserva espacios y saltos de línea del contenido. |
| `<blockquote>` | Representa una cita extensa. |
| `<q>` | Representa una cita breve. |
| `<cite>` | Identifica el título de una obra citada. |
| `<br>` | Introduce un salto de línea. |
| `<hr>` | Representa una separación temática. |

### Ejemplos:

```html
<h1>Título principal</h1>

<h2>Subtítulo</h2>

<p>Este es un párrafo de ejemplo.</p>

<strong>Texto importante</strong>

<em>Texto enfatizado</em>

<mark>Texto resaltado</mark>

<p>Fórmula química: H<sub>2</sub>O</p>

<p>Potencia matemática: 5<sup>2</sup></p>

<blockquote>
    El conocimiento se construye mediante la práctica.
</blockquote>

<pre>
    Línea 1
    Línea 2
    Línea 3
</pre>
```

---

## 7. ENCABEZADOS Y SECCIONES

Los encabezados permiten establecer una jerarquía dentro del contenido.

### Jerarquía de encabezados

| Etiqueta | Función |
|---|---|
| `<h1>` | Encabezado principal. |
| `<h2>` | Encabezado de segundo nivel. |
| `<h3>` | Encabezado de tercer nivel. |
| `<h4>` | Encabezado de cuarto nivel. |
| `<h5>` | Encabezado de quinto nivel. |
| `<h6>` | Encabezado de sexto nivel. |

### Ejemplo:

```html
<h1>Desarrollo web</h1>

<h2>HTML</h2>

<h3>Estructura básica</h3>

<h4>Elementos principales</h4>

<h5>Etiquetas</h5>

<h6>Ejemplos</h6>
```

Los encabezados deben utilizarse para organizar jerárquicamente el contenido, no simplemente para cambiar el tamaño del texto.

---

## 8. ELEMENTOS SEMÁNTICOS

Los elementos semánticos describen el significado y la función del contenido dentro de una página web.

Facilitan la comprensión de la estructura del documento por parte de los navegadores, motores de búsqueda y tecnologías de asistencia.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<header>` | Representa la cabecera de una página o sección. |
| `<nav>` | Agrupa enlaces de navegación. |
| `<main>` | Contiene el contenido principal del documento. |
| `<section>` | Agrupa contenido relacionado dentro de una sección. |
| `<article>` | Representa contenido independiente y autónomo. |
| `<aside>` | Contiene información complementaria. |
| `<footer>` | Representa el pie de página o sección. |
| `<address>` | Proporciona información de contacto. |
| `<figure>` | Agrupa contenido independiente, como imágenes o diagramas. |
| `<figcaption>` | Proporciona una descripción o título para un elemento `<figure>`. |
| `<time>` | Representa una fecha u hora. |
| `<details>` | Crea un elemento desplegable de información. |
| `<summary>` | Define el encabezado visible de un elemento `<details>`. |

### Ejemplo de estructura semántica:

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <title>Mi sitio web</title>
</head>

<body>

    <header>
        <h1>Mi página web</h1>

        <nav>
            <a href="#inicio">Inicio</a>
            <a href="#servicios">Servicios</a>
            <a href="#contacto">Contacto</a>
        </nav>
    </header>

    <main>

        <section id="inicio">
            <h2>Bienvenido</h2>
            <p>Contenido principal de la página.</p>
        </section>

        <section id="servicios">
            <h2>Servicios</h2>

            <article>
                <h3>Desarrollo web</h3>
                <p>Información sobre nuestros servicios.</p>
            </article>
        </section>

        <aside>
            <h2>Información adicional</h2>
            <p>Contenido complementario.</p>
        </aside>

    </main>

    <footer id="contacto">
        <p>Todos los derechos reservados.</p>
    </footer>

</body>
</html>
```

---

## 9. ENLACES Y RUTAS

Los enlaces permiten conectar documentos, páginas y recursos mediante la etiqueta `<a>`.

### Etiqueta principal

```html
<a href="https://www.google.com">Visitar Google</a>
```

### Atributos de los enlaces

| Atributo | Función |
|---|---|
| `href` | Define la dirección de destino. |
| `target` | Define dónde se abre el enlace. |
| `rel` | Establece la relación entre el documento actual y el destino. |
| `download` | Indica que el recurso debe descargarse. |
| `title` | Proporciona información adicional. |

### Tipos de rutas

**1. Ruta absoluta**

Contiene la dirección completa del recurso.

```html
<a href="https://www.ejemplo.com">Página externa</a>
```

**2. Ruta relativa**

Indica la ubicación del recurso respecto al documento actual.

```html
<a href="contacto.html">Contacto</a>
```

**3. Ruta a un directorio**

```html
<img src="imagenes/logo.png" alt="Logo">
```

**4. Ruta a una sección del documento**

```html
<a href="#contacto">Ir a contacto</a>

<section id="contacto">
    <h2>Contacto</h2>
</section>
```

**5. Enlace de correo electrónico**

```html
<a href="mailto:correo@ejemplo.com">Enviar correo</a>
```

**6. Enlace telefónico**

```html
<a href="tel:+34123456789">Llamar</a>
```

---

## 10. LISTAS

HTML permite organizar información mediante diferentes tipos de listas.

### Lista desordenada

Se utiliza cuando el orden de los elementos no es importante.

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
</ul>
```

- `<ul>`: define una lista desordenada.
- `<li>`: representa cada elemento de la lista.

### Lista ordenada

Se utiliza cuando existe una secuencia o jerarquía de elementos.

```html
<ol>
    <li>Instalar el editor</li>
    <li>Crear el documento</li>
    <li>Escribir el código</li>
</ol>
```

### Atributos de listas ordenadas

| Atributo | Función |
|---|---|
| `type` | Define el tipo de numeración. |
| `start` | Define el número inicial. |
| `reversed` | Invierte el orden de numeración. |

### Lista de definiciones

Se utiliza para presentar términos y sus respectivas descripciones.

```html
<dl>
    <dt>HTML</dt>
    <dd>Lenguaje de marcado para estructurar páginas web.</dd>

    <dt>CSS</dt>
    <dd>Lenguaje utilizado para definir la presentación visual.</dd>
</dl>
```

- `<dl>`: define la lista de descripciones.
- `<dt>`: define un término.
- `<dd>`: proporciona su descripción.

---

## 11. TABLAS

Las tablas permiten organizar información en filas y columnas.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<table>` | Define una tabla. |
| `<caption>` | Proporciona un título o descripción a la tabla. |
| `<thead>` | Agrupa las filas de encabezado. |
| `<tbody>` | Agrupa las filas del cuerpo. |
| `<tfoot>` | Agrupa las filas de resumen o pie. |
| `<tr>` | Define una fila. |
| `<th>` | Define una celda de encabezado. |
| `<td>` | Define una celda de datos. |
| `<colgroup>` | Agrupa columnas para aplicar características comunes. |
| `<col>` | Representa una columna dentro de un grupo. |

### Ejemplo:

```html
<table>

    <caption>Lenguajes de programación</caption>

    <thead>
        <tr>
            <th>Lenguaje</th>
            <th>Tipo</th>
            <th>Uso</th>
        </tr>
    </thead>

    <tbody>
        <tr>
            <td>PHP</td>
            <td>Programación</td>
            <td>Desarrollo backend</td>
        </tr>

        <tr>
            <td>HTML</td>
            <td>Marcado</td>
            <td>Estructura web</td>
        </tr>
    </tbody>

</table>
```

### Atributos importantes

| Atributo | Función |
|---|---|
| `colspan` | Permite que una celda ocupe varias columnas. |
| `rowspan` | Permite que una celda ocupe varias filas. |
| `scope` | Define el alcance de una celda de encabezado. |

### Ejemplo de combinación de celdas

```html
<table>
    <tr>
        <th colspan="2">Información personal</th>
    </tr>

    <tr>
        <td>Nombre</td>
        <td>Juan</td>
    </tr>
</table>
```

---

## 12. FORMULARIOS

Los formularios permiten recopilar información introducida por los usuarios y enviarla para su procesamiento.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<form>` | Define un formulario. |
| `<fieldset>` | Agrupa controles relacionados. |
| `<legend>` | Define el título de un grupo `<fieldset>`. |
| `<label>` | Proporciona una etiqueta descriptiva a un control. |
| `<input>` | Crea diferentes tipos de controles de entrada. |
| `<textarea>` | Permite introducir texto en varias líneas. |
| `<button>` | Define un botón. |
| `<select>` | Crea una lista de opciones seleccionables. |
| `<option>` | Define una opción dentro de una lista. |
| `<optgroup>` | Agrupa opciones relacionadas. |
| `<datalist>` | Proporciona sugerencias para un campo de entrada. |
| `<output>` | Representa el resultado de un cálculo o acción. |

### Ejemplo de formulario:

```html
<form action="/procesar" method="POST">

    <fieldset>

        <legend>Datos personales</legend>

        <label for="nombre">Nombre:</label>
        <input
            type="text"
            id="nombre"
            name="nombre"
            required
        >

        <br><br>

        <label for="correo">Correo electrónico:</label>
        <input
            type="email"
            id="correo"
            name="correo"
            required
        >

        <br><br>

        <label for="edad">Edad:</label>
        <input
            type="number"
            id="edad"
            name="edad"
            min="18"
        >

        <br><br>

        <label for="mensaje">Mensaje:</label>
        <textarea
            id="mensaje"
            name="mensaje"
            rows="4"
            maxlength="300"
        ></textarea>

        <br><br>

        <label for="pais">País:</label>

        <select id="pais" name="pais">
            <option value="es">España</option>
            <option value="co">Colombia</option>
            <option value="mx">México</option>
        </select>

        <br><br>

        <button type="submit">Enviar</button>

    </fieldset>

</form>
```

### Tipos de input

| Tipo | Función |
|---|---|
| `text` | Entrada de texto. |
| `password` | Entrada de contraseña. |
| `email` | Entrada de correo electrónico. |
| `number` | Entrada numérica. |
| `tel` | Entrada de número telefónico. |
| `url` | Entrada de direcciones web. |
| `date` | Selección de fecha. |
| `time` | Selección de hora. |
| `datetime-local` | Selección de fecha y hora local. |
| `checkbox` | Casilla de selección múltiple. |
| `radio` | Selección de una opción entre varias. |
| `file` | Selección de archivos. |
| `color` | Selector de color. |
| `range` | Selector de valores dentro de un rango. |
| `submit` | Botón para enviar el formulario. |
| `reset` | Restablece los valores del formulario. |
| `hidden` | Campo que no se muestra visualmente. |
| `search` | Campo destinado a búsquedas. |

### Atributos de formularios

| Atributo | Función |
|---|---|
| `action` | Define dónde se envían los datos. |
| `method` | Define el método de envío. |
| `name` | Identifica el campo enviado. |
| `value` | Define el valor del control. |
| `placeholder` | Muestra una indicación dentro del campo. |
| `required` | Hace obligatorio completar el campo. |
| `maxlength` | Establece la cantidad máxima de caracteres. |
| `minlength` | Establece la cantidad mínima de caracteres. |
| `min` | Define el valor mínimo. |
| `max` | Define el valor máximo. |
| `pattern` | Define un patrón de validación. |
| `checked` | Marca inicialmente una casilla o botón de opción. |
| `selected` | Selecciona inicialmente una opción. |
| `multiple` | Permite seleccionar varios valores cuando el control lo admite. |
| `disabled` | Deshabilita el control. |
| `readonly` | Impide modificar el valor del control. |

### Métodos de envío

- `GET`: envía los datos mediante parámetros en la URL.
- `POST`: envía los datos en el cuerpo de la solicitud HTTP.

**Importante:** HTML permite realizar validaciones básicas en el navegador, pero la validación y seguridad de los datos también deben realizarse en el servidor.

---

## 13. ELEMENTOS MULTIMEDIA

HTML permite incorporar imágenes, vídeos y archivos de audio directamente en una página web.

### Imágenes

La etiqueta `<img>` permite incorporar imágenes.

```html
<img
    src="imagenes/foto.jpg"
    alt="Descripción de la imagen"
    width="400"
>
```

Atributos principales:

- `src`: ubicación de la imagen.
- `alt`: descripción alternativa.
- `width`: ancho.
- `height`: altura.
- `loading`: permite configurar la carga de la imagen, por ejemplo, `lazy`.

### Vídeos

La etiqueta `<video>` permite reproducir archivos de vídeo.

```html
<video width="500" controls>

    <source src="videos/video.mp4" type="video/mp4">

    Tu navegador no puede reproducir este vídeo.

</video>
```

Atributos principales:

- `controls`: muestra los controles de reproducción.
- `autoplay`: permite iniciar automáticamente la reproducción.
- `muted`: silencia el audio.
- `loop`: repite el vídeo.
- `poster`: define una imagen de portada.
- `width`: establece el ancho.
- `height`: establece la altura.

### Audio

La etiqueta `<audio>` permite reproducir archivos de sonido.

```html
<audio controls>

    <source src="audio/musica.mp3" type="audio/mpeg">

    Tu navegador no puede reproducir este audio.

</audio>
```

Atributos principales:

- `controls`: muestra los controles.
- `autoplay`: permite la reproducción automática.
- `muted`: silencia el audio.
- `loop`: repite la reproducción.

---

## 14. CONTENIDO INCRUSTADO

Permite incorporar recursos externos o documentos dentro de una página HTML.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<iframe>` | Incrusta otro documento HTML dentro de la página actual. |
| `<object>` | Representa un recurso externo. |
| `<embed>` | Incrusta contenido externo. |
| `<picture>` | Permite ofrecer diferentes versiones de una imagen. |
| `<source>` | Define recursos alternativos para elementos multimedia. |
| `<canvas>` | Proporciona un área de dibujo controlada mediante JavaScript. |
| `<svg>` | Permite incorporar gráficos vectoriales escalables. |

### Ejemplo de iframe

```html
<iframe
    src="https://www.ejemplo.com"
    width="600"
    height="400"
    title="Página incrustada"
></iframe>
```

### Ejemplo de picture

```html
<picture>

    <source
        media="(max-width: 600px)"
        srcset="imagenes/movil.jpg"
    >

    <img
        src="imagenes/escritorio.jpg"
        alt="Imagen adaptable"
    >

</picture>
```

### Ejemplo de canvas

```html
<canvas id="miCanvas" width="300" height="150"></canvas>
```

El elemento `<canvas>` necesita JavaScript para dibujar contenido mediante su contexto gráfico.

---

## 15. ELEMENTOS DE AGRUPACIÓN

Permiten agrupar contenido y organizar elementos dentro del documento.

### Etiquetas principales

| Etiqueta | Función |
|---|---|
| `<div>` | Contenedor genérico de bloque. |
| `<span>` | Contenedor genérico en línea. |
| `<figure>` | Agrupa contenido independiente. |
| `<figcaption>` | Describe el contenido de un `<figure>`. |
| `<details>` | Crea un bloque de información desplegable. |
| `<summary>` | Define el título de un bloque desplegable. |

### Diferencia entre div y span

**Div:** se utiliza normalmente para agrupar elementos en bloques.

```html
<div class="contenedor">
    <h2>Desarrollo web</h2>
    <p>Aprendiendo HTML y CSS.</p>
</div>
```

**Span:** se utiliza para agrupar fragmentos de contenido en línea.

```html
<p>
    Estoy aprendiendo
    <span class="destacado">HTML</span>.
</p>
```

### Elemento details

```html
<details>
    <summary>¿Qué es HTML?</summary>
    <p>Es un lenguaje de marcado utilizado para estructurar páginas web.</p>
</details>
```

---

## 16. CARACTERES ESPECIALES Y ENTIDADES HTML

Las entidades HTML permiten representar caracteres reservados, símbolos y caracteres especiales dentro de un documento.

### Entidades frecuentes

| Entidad | Resultado | Función |
|---|---|---|
| `&lt;` | < | Representa el símbolo menor que. |
| `&gt;` | > | Representa el símbolo mayor que. |
| `&amp;` | & | Representa el símbolo ampersand. |
| `&quot;` | " | Representa las comillas dobles. |
| `&apos;` | ' | Representa el apóstrofo. |
| `&nbsp;` | Espacio | Representa un espacio no separable. |
| `&copy;` | © | Símbolo de copyright. |
| `&reg;` | ® | Símbolo de marca registrada. |
| `&euro;` | € | Símbolo del euro. |

### Ejemplo:

```html
<p>HTML utiliza etiquetas como &lt;html&gt; y &lt;body&gt;.</p>

<p>Todos los derechos reservados &copy; 2026.</p>
```

---

## 17. COMENTARIOS EN HTML

Los comentarios permiten escribir anotaciones dentro del código fuente sin que aparezcan como contenido visible de la página.

### Sintaxis:

```html
<!-- Este es un comentario en HTML -->

<h1>Mi página web</h1>
```

### Utilidad

- Documentar fragmentos de código.
- Identificar secciones.
- Facilitar el mantenimiento.
- Dejar anotaciones para otros desarrolladores.

**Importante:** los comentarios pueden visualizarse al inspeccionar el código fuente, por lo que no deben utilizarse para almacenar contraseñas, claves o información confidencial.

---

## 18. INTEGRACIÓN CON CSS Y JAVASCRIPT

HTML puede trabajar conjuntamente con CSS y JavaScript para construir páginas web completas.

### HTML + CSS

CSS permite definir la presentación visual de los elementos HTML.

```html
<head>
    <link rel="stylesheet" href="estilos.css">
</head>
```

También es posible utilizar CSS directamente dentro del documento:

```html
<style>
    body {
        background-color: #222;
        color: white;
    }
</style>
```

### HTML + JavaScript

JavaScript permite añadir interactividad y modificar el contenido de una página.

```html
<head>
    <script src="script.js" defer></script>
</head>
```

También se puede incorporar código directamente:

```html
<script>
    console.log("Hola desde JavaScript");
</script>
```

### Ejemplo de integración

```html
<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <title>Integración web</title>

    <link rel="stylesheet" href="estilos.css">

    <script src="script.js" defer></script>
</head>

<body>

    <h1 id="titulo">Mi primera página</h1>

    <button id="boton">Cambiar título</button>

</body>
</html>
```

---

## 19. ACCESIBILIDAD Y BUENAS PRÁCTICAS

La accesibilidad permite que las páginas web puedan ser utilizadas por personas con diferentes necesidades y tecnologías de asistencia.

### Buenas prácticas

1. Declarar el idioma del documento mediante `lang`.
2. Utilizar una estructura correcta de encabezados.
3. Incorporar el atributo `alt` en las imágenes.
4. Utilizar etiquetas semánticas cuando corresponda.
5. Asociar cada campo de formulario con su etiqueta `<label>`.
6. Utilizar textos descriptivos en los enlaces.
7. Mantener una estructura clara y ordenada.
8. Evitar utilizar elementos HTML únicamente para modificar la apariencia.
9. Comprobar que los formularios puedan utilizarse mediante teclado.
10. Validar el código HTML.

### Ejemplo correcto de accesibilidad en un formulario

```html
<label for="usuario">Nombre de usuario:</label>

<input
    type="text"
    id="usuario"
    name="usuario"
    required
>
```

El atributo `for` del elemento `<label>` debe coincidir con el `id` del control asociado.

### Validación HTML

Puedes comprobar la estructura de tus documentos mediante el validador oficial:

https://validator.w3.org/

---

## 20. ESTRUCTURA DE UN PROYECTO HTML

Una estructura organizada facilita el desarrollo y mantenimiento de los proyectos web.

### Ejemplo de organización

```text
PROYECTO-WEB/
│
├── index.html
│
├── pages/
│   ├── contacto.html
│   └── servicios.html
│
├── css/
│   └── estilos.css
│
├── js/
│   └── script.js
│
├── images/
│   ├── logo.png
│   └── banner.jpg
│
└── assets/
    └── iconos/
```

### Descripción de los archivos

| Archivo o directorio | Función |
|---|---|
| `index.html` | Documento principal del proyecto. |
| `pages/` | Contiene otras páginas HTML. |
| `css/` | Almacena hojas de estilos. |
| `js/` | Contiene archivos JavaScript. |
| `images/` | Almacena imágenes. |
| `assets/` | Contiene recursos adicionales. |

### Ejemplo de conexión de archivos

Desde `index.html`:

```html
<link rel="stylesheet" href="css/estilos.css">

<script src="js/script.js" defer></script>

<img src="images/logo.png" alt="Logo del proyecto">
```

---

## 📚 RECURSOS DE CONSULTA

- [Documentación HTML — MDN Web Docs](https://developer.mozilla.org/es/docs/Web/HTML)
- [HTML Living Standard — WHATWG](https://html.spec.whatwg.org/)
- [Validador HTML — W3C](https://validator.w3.org/)

---

## 🎯 OBJETIVO DEL REPOSITORIO

Construir una referencia organizada de HTML que permita consultar sus etiquetas, atributos y estructuras fundamentales, reforzando los conocimientos necesarios para el desarrollo web.

**Aprendiendo · Practicando · Construyendo.**
