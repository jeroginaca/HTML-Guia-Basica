![Bienvenidos](https://i.ibb.co/sy4DPv5/guia-basica-html.png)
# Bienvenidos a mi Guía Básica de HTML - 2023

Este año voy a empezar a compartir contenido educativo 🤓

Descubrí la programación el año pasado y me metí de lleno a estudiarla, ahora siento que es momento de compartir lo que he aprendido.

> En esta Guía vamos a ver los principios de HTML, desde lo más básico, hasta llegar a los estilos CSS.

🔥

## 1. Introducción al HTML

El **html** es la estructura y contenido de nuestra web. Es es el archivo principal a partir del cual se llaman el resto de archivos que necesitamos para visualizar nuestra web, tales como las hojas de estilo, imágenes, etc.

### ¿Cómo funciona exactamente?
Las elementos **HTML** se escriben con los símbolos **< >**  para abrir, y **</ >**  para cerrar.
```html
<etitqueta> </etiqueta>
```
Nuestro archivo HTML va a tener varios tipos de eituqetas, de docuemnto, de bloque, de imagen, de enlace, etc. También estas pueden tener atributos, pero arranquemos con lo primero que encontramos en nuestro archivo HTML: **Las Etiquetas de Documento**

```html
<!DOCTYPE html>
<head>
    <meta charset="UTF-8">
    <title>Guía Básica de HTML</title>
</head>
<body>
    
</body>
</html>
```

---

## 2. Etiquetas HTML de documento

Vamos a enumerar las distintas etiquetas que se utilizan y describir sus funciones.

```html
<!DOCTYPE html> 
```

Indica al navegador que la web sigue los estándares y debe ser renderizada como tal. Se pone al principio del documento html y no se cierra.

```html
<html></html>
```
Etiqueta que engloba el resto del documento.

```html
<head></head>
```

Etiqueta con información para el navegador diferente del contenido: título de la
página, hoja de estilos, codificado, etc.

```html
<body></body>
```
Contenido (texto, imágenes, etc) de la página.

```html
<title></title>
```
Título de la página, que suele figurar en los resultados de búsqueda o en la pestaña del navegador.

```html
<meta charset="utf-8">
```
Codifica caracteres especiales.

---


## 3. Etiquetas HTML de Texto

```html
<p></p>
```
Marca un párrafo.

```html
<h1></h1>
```
Marca un encabezado de primer nivel. Solo puede haber uno por página.

```html
<h2></h2>
```
Marca un encabezado de segundo nivel.

```html
<h3></h3>
```
Marca un encabezado de tercer nivel.

```html
<h4></h4>
```
Marca un encabezado de cuarto nivel.

```html
<h5></h5>
```

Marca un encabezado de quinto nivel.

```html
<h6></h6>
```
Marca un encabezado de sexto nivel.

```html
<!—- comentario -—>
``` 
Para introducir comentarios o comentar cierta parte del código

```html
<br> 
``` 
Marca un salto de línea. No requiere de cierre.

```html
<em></em>
```
Etiqueta semántica para hacer énfasis en una palabra en particular. Se renderiza como una cursiva.

```html
<strong></strong>
```

Etiqueta semántica para indicar la relevancia en un texto de una palabra en particular. Se renderiza como una negrita.

```html
<span></span>
```
Etiqueta sin valor semántico que sirve para acotar trozos de texto.

---

## 4. Etiquetas HTML de Bloque

```html
<div></div>
```
Etiqueta sin valor semántico que nos permite agrupar bloques.

```html
<ul></ul>
```
Etiqueta de listado no ordenado. Solo puede contener elementos de lista (< li >). 

```html
<li></li>
```
Etiqueta de elemento de lista. Puede contener cualquier tipo de elemento html.

```html
<ol></ol>
```
Etiqueta de listado ordenado. Solo puede contener elementos de lista (< li >).

---

## 5. Atributos para las etiquetas html

Los atributos nos sirven para diferenciar a nuestros elementos cuando querramos darles estilos. Se escriben en la etiqueta de apertura de un elemento, después del nombre y se pueden escribir varios atributos separados por espacios. 

La forma de asignar un valor a un atributo es con el símbolo `=` y el valor entre comillas. No puede haber espacios entre el atributo y el `=`, o entre el `=` y las comillas.

**Ejemplo:** `<div class="ejemplo" id="ejemplo">`

```html
class=" "
```
Asigna una o más clases a un elemento html. Si hay más de una clase, se separan con espacios.

```html
id=" "
```
Asigna un identificador único a un elemento html. Un elemento **no puede tener más de un id**, y **no puede haber dos elementos con el mismo id.**

---

## 6. Etiquetas HTML de imágenes y enlaces

**Rutas de archivo**

Cuando querramos mostrar un archivo por ejemplo de imagen, debemos llamarlo por su nombre y exstensión, y buscarlo en la carpeta que lo contenga.

Para navegar entre carpetas se utiliza `.` seguido por `/` y ahí el nombre de la carpeta. En caso que la carpeta estuviese en otro nivel colcamos `../` y si queremos subir otro nivel más `../../carpeta` Para navegar entre carpetas las separamos por `/` hasta llegar a nuestro archivo.
**Ejamplo:** `../../imagenes/background.jpg`

**Etiqueta de imagen**
```html
<img src=" " alt=" ">
```
 El atributo src indica la ruta de la imagen, y el alt es el texto alternativo que se mostrara en caso que la imagen no cargue.
 
 Para controlar el tamaño de nuestra imagen podemos utilizar el atributo `width=""`
 **Ejemplo:**
 ```html
    <img src="./img/portada.png" width="60%">
```

**Etiqueta de enlace**
```html
<a href=" "></a>
```
El atributo href indica la página de destino. Puede ser a un archivo dentro de nuestro proyecto, o a un sitio web (en este caso hay que poner la URL **completa**, con http://).

Un enlace puede ser a una sección de la misma página, marcada con un id. En ese caso, el href empezará con `#` y el nombre del id.

Para abrir un enlace en una ventana nueva, añadiremos el atributo `target= ̋_blank ̋` 

---

## 7. Enlaces de mail y teléfono

Cuando querramos colocar un email o un telefono dentro de nuestra etiqueta de enlace `<a>` debemos tener en cuenta lo siguiente:

```html
<a href="mailto:un@email.com">un@email.com</a>
```
Para un email debemos agregar `mailto:` y nuestra dirección de correo. Entonces cuando el usuario haga click podra mandarnos un mail instantaneamente.

```html
<a href="tel:+34666666666">666 666 666</a>
```
Para llamar a un telefono agregamos `tel:` seguido de el numero completo con caracteristica de país y sin espacios.

---

## 8. BONUS TRACK: 
### BOTONES
```html
<button>
```

La etiqueta `<button>` en HTML se utiliza para crear un botón, que puede ser utilizado para enviar un formulario, realizar una acción o simplemente como un enlace a otra página o sección de la misma.

```html
<button>Haz clic aquí</button>
```

A los botones podemos agregarles atributos por ejemplo, el atributo `type` puede ser utilizado para especificar el tipo de botón (por ejemplo, submit para enviar un formulario). También podemos darle atributos que ejecuten funciones Javascript como `onClick()`.

Pero por el momento los botones los vamos a utilizar para navegar entre enlaces.

### IFRAME

La etiqueta `<iframe>` se utiliza para insertar un documento HTML dentro de otro documento HTML. Es decir, nos permite mostrar una página web dentro de otra.

```html
<iframe src="https://www.google.com"></iframe>
```
También podemos agregarle atributos `width=""` y `heigth=""` para controlar sus dimensiones.

**Ejemplo:**
```html
<iframe src="https://www.google.com" width="400px" height="300px"></iframe>
```

---

🔥

## ¡Esto Fue todo por ahora!

Hasta acá llegamos con La Guía Básica de HTML5 🎉

>El que quiera corregir algún error de tipeo, agregar algo, o lo que sea puede hacerlo y con gusto aceptare el Request!

**Muchas gracias por llegar hasta aquí**
---

## Contacto

- 😀 Para ver mis trabajos visita [mi portfolio](https://www.jeronimoginaca.com)
- 👔 LinkedIn: [Jerónimo Ginaca](https://www.linkedin.com/in/jeronimoginaca/)
- 📨 Email: [jeroginaca@gmail.com](mailto:jeroginaca@gmail.com)
- 📲 Whatsapp: [click here](https://wa.me/5491126343056)

