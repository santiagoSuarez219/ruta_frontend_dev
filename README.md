## Tabla de contenido

- [Modulo 1: Fundamentos de HTML y CSS](#modulo-1-fundamentos-de-html-y-css)
  - [HTML](#html)
    - [Para que sirven las herramientas del navegador](#para-que-sirven-las-herramientas-del-navegador)
  - [Motores de renderizado: de archivos a pixeles](#motores-de-renderizado-de-archivos-a-pixeles)
    - [Proceso de renderizado del motor del navegador](#proceso-de-renderizado-del-motor-del-navegador)
  - [Anatomia de un documento HTML y sus elementos](#anatomia-de-un-documento-html-y-sus-elementos)
  - [Atributos HTML](#atributos-html)
  - [Elementos anidados](#elementos-anidados)
  - [Elementos vacios en HTML](#elementos-vacios-en-html)
  - [Estructura basica de un documento HTML](#estructura-basica-de-un-documento-html)
  - [Comentarios de HTML](#comentarios-de-html)
  - [HTML Semantico](#html-semantico)
    - [Etiquetas semanticas](#etiquetas-semanticas)
    - [El problema con la etiqueta div](#el-problema-con-la-etiqueta-div)
    - [Ventajas](#ventajas)
  - [Etiquetas HTML mas usadas](#etiquetas-html-mas-usadas)
  - [Etiquetas de layaout o diseño de pagina](#etiquetas-de-layaout-o-diseño-de-pagina)
  - [Etiquetas de enlace](#etiquetas-de-enlace)
  - [Etiquetas para textos](#etiquetas-para-textos)
  - [Etiquetas para listas](#etiquetas-para-listas)
  - [Etiquetas para multimedia](#etiquetas-para-multimedia)
  - [Etiquetas para formularios](#etiquetas-para-formularios)
  - [CSS](#css)
  - [Anatomia de una declaracion CSS: selectores, propiedades y valores](#anatomia-de-una-declaracion-css-selectores-propiedades-y-valores)
    - [Declaraciones](#declaraciones)
  - [Algunas propiedades inciales](#algunas-propiedades-inciales)
  - [Medidas inciales en CSS](#medidas-inciales-en-css)
  - [Comentarios en CSS](#comentarios-en-css)
  - [Selectores de CSS](#selectores-de-css)
    - [Selectores de tipo](#selectores-de-tipo)
    - [Selectores de clase](#selectores-de-clase)
    - [Selectores de id](#selectores-de-id)
    - [Selectores de atributo](#selectores-de-atributo)
    - [Selectores combinados](#selectores-combinados)
    - [Combinador descendientes](#combinador-descendientes)
    - [Combinador de hijo directo](#combinador-de-hijo-directo)
    - [Combinador de hermanos adyacentes](#combinador-de-hermanos-adyacentes)
    - [Combinador de hermanos generales](#combinador-de-hermanos-generales)
  - [Pseudoclases y pseudoelementos](#pseudoclases-y-pseudoelementos)
    - [Pseudoclases](#pseudoclases)
  - [Pseudoelementos](#pseudoelementos)
  - [Cascada y especificidad en CSS](#cascada-y-especificidad-en-css)
  - [Estilos en linea](#estilos-en-linea)
  - [Especificidad en selectores](#especificidad-en-selectores)
  - [Tipos de displays mas usados](#tipos-de-displays-mas-usados)
    - [Block](#block)
    - [Visualizacion en linea (inline)](#visualizacion-en-linea-inline)
    - [Visualizacion de bloque y linea (inline - block)](#visualizacion-de-bloque-y-linea-inline---block)
    - [Visualizacion nula (none)](#visualizacion-nula-none)
  - [Flexbox y CSS Grid](#flexbox-y-css-grid)
    - [Flexbox](#flexbox)
    - [Grid](#grid)
  - [Modelo de caja](#modelo-de-caja)
  - [Content](#content)
  - [Border](#border)
  - [Padding](#padding)
  - [Margin](#margin)
  - [Valores por defecto](#valores-por-defecto)
  - [El tamanio total del elemento](#el-tamanio-total-del-elemento)
  - [Propiedad box-sizing](#propiedad-box-sizing)
    - [Problema con el tamaño de los bordes](#problema-con-el-tamaño-de-los-bordes)
  - [Colapso de margenes](#colapso-de-margenes)
  - [Posicionamiento en CSS](#posicionamiento-en-css)
    - [Propiedades de posicion](#propiedades-de-posicion)
  - [Posicion fija](#posicion-fija)
  - [Posicion variable fija](#posicion-variable-fija)
  - [Z - index y el contexto de apilamiento](#z---index-y-el-contexto-de-apilamiento)
  - [Propiedades y valores de CSS mas usados](#propiedades-y-valores-de-css-mas-usados)
  - [Bordes redondeados](#bordes-redondeados)
  - [Unidades de medida](#unidades-de-medida)
    - [Medidas absolutas](#medidas-absolutas)
    - [Medidas relativas](#medidas-relativas)
    - [Diferencias entre porcentajes y la anchura y altura de la pantalla](#diferencias-entre-porcentajes-y-la-anchura-y-altura-de-la-pantalla)
  - [Responsive Design](#responsive-design)
    - [media queries](#media-queries)
    - [Estructura](#estructura)
- [Modulo 2: Tailwind CSS](#modulo-2-tailwind-css)
  - [Mobile first](#mobile-first)
  - [Utility first (framework basado en utilidades)](#utility-first-framework-basado-en-utilidades)
  - [Directivas de tailwindcss](#directivas-de-tailwindcss)
  - [Paleta de colores](#paleta-de-colores)
    - [Enlaces de interes](#enlaces-de-interes)
  - [Medidas y breakpoints](#medidas-y-breakpoints)
    - [Width](#width)
    - [Height](#height)
    - [Breakpoints](#breakpoints)
  - [Flexbox](#flexbox-1)
    - [Algunas propiedades interesantes de flexbox](#algunas-propiedades-interesantes-de-flexbox)
  - [Plugins oficiales de Tailwind CSS](#plugins-oficiales-de-tailwind-css)
  - [Aplicacion Platzi Travel](#aplicacion-platzi-travel)
    - [Enlaces de interes](#enlaces-de-interes-1)
  - [Design System](#design-system)
  - [Practica: Seccion Home Mobile](#practica-seccion-home-mobile)
  - [Practica: Componentes card mobile](#practica-componentes-card-mobile)
  - [Extraccion de componentes a clases](#extraccion-de-componentes-a-clases)
  - [Practica: seccion recomendados mobile](#practica-seccion-recomendados-mobile)
  - [Animaciones con tailwind](#animaciones-con-tailwind)
  - [Focus](#focus)
    - [Focus within](#focus-within)
  - [Ring](#ring)
  - [Practica: seccion rentas destacadas](#practica-seccion-rentas-destacadas)
  - [Practica: seccion preguntas frecuentes](#practica-seccion-preguntas-frecuentes)
  - [Practica: seccion footer](#practica-seccion-footer)
  - [Practica: TabBar](#practica-tabbar)
  - [Practica: responsive design](#practica-responsive-design)
  - [Practica: creando la navbar](#practica-creando-la-navbar)
  - [Dark mode](#dark-mode)
  - [Preparando para produccion](#preparando-para-produccion)
  - [Migrar desde tailwindcss 2.x a 3.x](#migrar-desde-tailwindcss-2x-a-3x)
- [Modulo 3: ReactJS](#modulo-3-reactjs)
  - [Enlaces de interes](#enlaces-de-interes-2)
  - [Que es ReactJS](#que-es-reactjs)
  - [Que es un componente](#que-es-un-componente)
  - [Que son Props](#que-son-props)
  - [Estilos con React](#estilos-con-react)
    - [Enlaces de interes](#enlaces-de-interes-3)
  - [Eventos con ReactJS](#eventos-con-reactjs)
    - [onClick](#onclick)
    - [onChange](#onchange)
  - [Estados](#estados)
    - [Practica: Estados](#practica-estados)
  - [Iconos](#iconos)
    - [Librerias de terceros](#librerias-de-terceros)
    - [Libreria de iconos personalizados](#libreria-de-iconos-personalizados)
  - [LocalStorage](#localstorage)
  - [Custom Hooks](#custom-hooks)
  - [Organizacion de archivos](#organizacion-de-archivos)
  - [Efectos en React](#efectos-en-react)
    - [useEffect](#useeffect)
    - [Practica: Implementando estados de carga y error en la aplicacion ToDos](#practica-implementando-estados-de-carga-y-error-en-la-aplicacion-todos)
  - [React Context](#react-context)
  - [React Portals](#react-portals)
  - [Formularios](#formularios)
  - [Deploy de la aplicacion en github pages](#deploy-de-la-aplicacion-en-github-pages)
  - [Versiones de React](#versiones-de-react)
  - [Creando proyectos de React](#creando-proyectos-de-react)
    - [create-react-app](#create-react-app)
    - [next.js](#nextjs)
- [Modulo 4: Ecoomerce con React, Vite y Tailwind](#modulo-4-ecoomerce-con-react-vite-y-tailwind)
  - [Enlaces de interes](#enlaces-de-interes-4)
  - [Vite](#vite)
  - [Instalacion de TailwindCSS](#instalacion-de-tailwindcss)
  - [Paginas del ecommerce](#paginas-del-ecommerce)
  - [Enrutamiento con React Router Dom](#enrutamiento-con-react-router-dom)
  - [Componente NavBar](#componente-navbar)
  - [Componente Layout](#componente-layout)
  - [Componente Card](#componente-card)
  - [Consumiendo una API](#consumiendo-una-api)
  - [Contexto global de la aplicacion](#contexto-global-de-la-aplicacion)
  - [Contador de productos en el carrito](#contador-de-productos-en-el-carrito)
  - [Abriendo el detalle de cada producto](#abriendo-el-detalle-de-cada-producto)
    - [Maquetacion e iconos](#maquetacion-e-iconos)
    - [Logica del componente](#logica-del-componente)
  - [Agregando el carrito de compras](#agregando-el-carrito-de-compras)
    - [SlideMenu del carrito de compras](#slidemenu-del-carrito-de-compras)
  - [Componente OrderCard](#componente-ordercard)
    - [Evitando duplicados en el carrito de compras](#evitando-duplicados-en-el-carrito-de-compras)
    - [Eliminar productos del carrito](#eliminar-productos-del-carrito)
    - [Total de la compra](#total-de-la-compra)
  - [Pagina MyOrders](#pagina-myorders)
  - [Pagina MyOrders](#pagina-myorders-1)
  - [Buscados de productos](#buscados-de-productos)
  - [Filtrando por categorias](#filtrando-por-categorias)
  - [Corrigiendo algunos bugs](#corrigiendo-algunos-bugs)
  - [Deploy de React en Netlify](#deploy-de-react-en-netlify)
- [Modulo 5: React con Typescript](#modulo-5-react-con-typescript)
  - [Creando una app con React y TypeScript](#creando-una-app-con-react-y-typescript)
  - [Diferentes formas de definir un componente.](#diferentes-formas-de-definir-un-componente)
  - [Props en TypeScript](#props-en-typescript)
  - [State con tipos primitivos](#state-con-tipos-primitivos)
  - [Tipos para eventos y callback de escuchadores](#tipos-para-eventos-y-callback-de-escuchadores)
- [Modulo 6: React Native](#modulo-6-react-native)
  - [Instalacion del CLI de React Native Expo](#instalacion-del-cli-de-react-native-expo)
  - [Instalacion de Android Studio para utilizar los emuladores](#instalacion-de-android-studio-para-utilizar-los-emuladores)
  - [Pruebas en un dispositivo fisico](#pruebas-en-un-dispositivo-fisico)
  - [Estructura de un proyecto](#estructura-de-un-proyecto)
  - [Creacion de componentes](#creacion-de-componentes)
  - [Propiedades entre componentes](#propiedades-entre-componentes)
  - [Propiedades por defecto](#propiedades-por-defecto)
  - [Instalando y configurando React Navigation](#instalando-y-configurando-react-navigation)
  - [Stack de navegacion](#stack-de-navegacion)
  - [Tab Navigation y SafeAreaView](#tab-navigation-y-safeareaview)
  - [Drawer Navigation](#drawer-navigation)
  - [Practica: Configuracion de React Navigation](#practica-configuracion-de-react-navigation)

# Modulo 1: Fundamentos de HTML y CSS

La web se construye mediante 3 tecnologías esenciales: HTML, CSS y JavaScript. Estos tres lenguajes son las bases en que una aplicación o página web está construida

## HTML

El lenguaje de marcado de hipertexto o HTML por sus siglas en inglés. (HyperText Markup Language) es el código para construir la estructura de una página web.

En otras palabras, HTML es el esqueleto con el cual definimos cada elemento que compone la página web, así como:

- Enlaces
- Párrafos
- Títulos
- Botones
- Imágenes
- Formulario

### Para que sirven las herramientas del navegador

Las herramientas del navegador son importantes para visualizar lo que ocurre con el código generado. Entre una de las opciones está identificar los elementos que están estructurados en la página web con sus respectivos estilos.

Las herramientas de desarrollador se despliegan con la combinación de teclas `F12 / Ctrl + Shift + I / Cmd + Opt  + I` o click derecho e "Inspeccionar" en tu navegador preferido. (Se recomienda Google Chrome )

## Motores de renderizado: de archivos a pixeles

Los motores de renderizado son programas que traducen nuestro código en un lenguaje que entiende el navegador, de esta manera el programa sabrá qué es lo que tiene que mostrar por pantalla al usuario.

Los navegadores tienen sus propios motores: Chrome - Blink, Edge - Edge HTML, Safari - Webkit y Firefox - Gecko. Todos realizan esta compilación de manera diferente, pero con el mismo resultado, es decir, convierte los archivos a píxeles.

### Proceso de renderizado del motor del navegador

El motor del navegador realiza 5 pasos o procesos para compilar nuestro código hasta el renderizado por pantalla. Estos pasos son los siguientes:

1. Transforma los archivos a un árbol de objetos HTML o CSS, estos se denominan DOM (Document Object Model) y CSSDOM (Cascade Style Sheet Object Model), respectivamente. Cada nodo en el árbol es una representación de los elementos que contiene el archivo HTML o CSS.
2. Calcula el estilo correspondiente a cada nodo del DOM relacionado al CSSDOM.
3. Calcula las dimensiones de cada nodo y dónde va en la pantalla.
4. Pinta o renderiza los diferentes elementos como cajas o contenedores.
5. Agrupa todas las cajas en diferentes capas para convertirlas en una imagen que se renderiza en pantalla.

## Anatomia de un documento HTML y sus elementos

Los elementos son cada una de las partes que conforman un archivo HTML. Su estructura contiene:

- Etiquetas: es la representación de un elemento HTML. Se divide en etiquetas de apertura, representadas por `<etiqueta>` y etiquetas de cierre, representadas por `</etiqueta>`
- Contenido: es el texto o elementos encerrados por la etiqueta, este valor es opcional en algunas de ellas.

```html
<h1>Hola mundo</h1>
```

## Atributos HTML

Los atributos HTML son propiedades en la etiqueta de apertura que manejan el comportamiento del elemento. Su valor está envuelto en comillas

```html
<h1 class="title">Hola mundo</h1>
```

## Elementos anidados

El anidamiento de elementos HTML consiste en envolver varias etiquetas en otras etiquetas. Interpreta a cada elemento HTML como una caja donde puedes guardar diferentes elementos u otras cajas. Estas cajas tendrán diferentes tamaños y estarán colocadas junto a otras.

```html
<section>
  <h1>Hola Mundo</h1>
  <p>Hola mundo desde HTML</p>
  <ul>
    <li>Elemento 1</li>
    <li>Elemento 2</li>
    <li>Elemento 3</li>
  </ul>
</section>
```

Aquellas etiquetas que envuelven a otras se las denomina “padres”. Es decir, `<section>` es padre de `<h1>, <p>, <ul>`, y a su vez `<ul>` es padre de 3 etiquetas `<li>`.

Las etiquetas que son el contenido de otras, se las denomina “hijos”. Es decir, las etiquetas `<h1>, <p>, <ul>` son hijos de `<section>`, y a su vez las etiquetas `<li>` son hijos de `<ul>`.

## Elementos vacios en HTML

Los elementos vacíos son aquellos que únicamente se representan en una etiqueta de apertura. Por ejemplo: `<img …>` . Estas etiquetas pueden cerrarse en la misma
etiqueta de apertura, utilizando la barra inclinada "/" al final `<img …/>`

```html
<img src="cat.jpg" />
```

## Estructura basica de un documento HTML

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body>
    <header></header>
    <nav></nav>
    <section></section>
    <footer></footer>
  </body>
</html>
```

1. Etiqueta Doctype: especifica que el archivo se maneje con la versión 5 de HTML.
2. Etiqueta html: Define el elemento raíz de un documento HTML. Todos los demás elementos deben estar contenidos dentro de este elemento raíz. En esta etiqueta se especifica el lenguaje de la página web mediante la propiedad lang.
3. Etiqueta head: Define la metainformación, es decir, toda información que no es contenido como tal de la página web. Por ejemplo, los enlaces a archivos CSS y JavaScript, el título y la imagen que aparecen en la pestaña del navegador. Esto es importante para motores de búsqueda como Google.
4. Etiqueta body: La etiqueta `<body>` define el contenido de la página web. Debe ser hijo cercano de `<html>` y padre de todas las etiquetas HTML, excepto por aquellas que definan metainformación.

## Comentarios de HTML

Los comentarios de HTML consisten en señalar algo que se ignorará. Para establecer un comentario HTML se lo envuelve entre `<!-- y -->`, independiente de la cantidad de líneas.

## HTML Semantico

El HTML semántico consiste en que cada elemento tenga su propia etiqueta que lo defina correctamente. Sin utilizar etiquetas muy generales, como `<div> o <span>`.

### Etiquetas semanticas

Las etiquetas semánticas para definir una interfaz de una página web son:

- `<Header>` define el encabezado de la página. (NO confundir con `<head>`).
- `<nav>` define una barra de navegación que incluye enlaces.
- `<section>` define una sección de la página.
- `<footer>` define un pie de página o de sección
- `<article>` define un artículo, el cual puede tener su propio encabezado, navegación, sección o pie de página.

### El problema con la etiqueta div

La etiqueta div define un bloque genérico de contenido, que no tiene ningún valor semántico. Se utiliza para elementos de diseño como contenedores.

### Ventajas

1. Ayuda a tu sitio a ser accesible
2. Mejora tu posicionamiento (SEO)
3. Código más claro, legible y mantenible
4. Ayuda a buscadores (como Google) a encontrar tu página.

## Etiquetas HTML mas usadas

Las etiquetas HTML más usadas son las siguientes, separadas en secciones comunes:

1. Header
2. Nav
3. Section
4. Article
5. Aside
6. Footer
7. Form
8. Input
9. Label
10. Button
11. H1 - H6
12. P
13. Span
14. Img
15. Svg
16. Iframe
17. Video

## Etiquetas de layaout o diseño de pagina

Las etiquetas más usadas para layout o diseño de página son aquellas que utilizamos para construir una página semántica.

```
<header>
<nav>
<section>
<article>
<aside>
<footer>
```

## Etiquetas de enlace

La etiqueta de enlace `<a>` o “anchor” define un vínculo o enlace hacia una URL. Se utiliza con el atributo href con el valor del enlace.

## Etiquetas para textos

Las etiquetas para textos son aquellas que nos permiten definir el contenido de la página web. Estas etiquetas son:

1. `<h1> - <h6>`
2. `<p>`
3. `<span>` define un contenedor genérico de tipo inline. Igual que `<div>` no tiene valor semántico y debes evitar su uso innecesario

## Etiquetas para listas

Las etiquetas para listas son aquellas que nos permiten definir listas de elementos. Estas etiquetas son:

1. `<ul>` define una lista desordenada
2. `<ol>` define una lista ordenada
3. `<li>` define un elemento de la lista

## Etiquetas para multimedia

Las etiquetas para multimedia son aquellas que nos permiten definir contenido multimedia. Estas etiquetas son:

1. `<img>` define una imagen
2. `<svg>` define una svg
3. `<iframe>` define un contenedor para una pagina web dentro de otra pagina web.
4. `<video>` define un contenedor de video

## Etiquetas para formularios

Las etiquetas para formularios son aquellas que nos permiten definir formularios. Estas etiquetas son:

1. `<form>` define un formulario
2. `<input>` define un elemento de entrada del formulario. Es necesario especificar el tipo con el atributo type. Existen varios tipos de input, revísalos en su [documentación](https://developer.mozilla.org/es/docs/Learn/Forms/HTML5_input_types).
3. `<label>` define un titulo para la etiqueta input. Es utilizado para acciones de accesibilidad.
4. `<button>` define un botón. Es usado para la interactividad de la página.

## CSS

El lenguaje de hojas de estilos en Cascada o CSS por sus siglas en inglés (Cascade Style Sheets) es el código para describir la presentación de los elementos de la página web, los que definimos con HTML

## Anatomia de una declaracion CSS: selectores, propiedades y valores

### Declaraciones

Una declaración de CSS es un bloque que especifica el conjunto de estilos que se añadirán a un elemento HTML. Su estructura contiene lo siguiente:

1. Selector: define el elemento o conjunto de elementos a los cuales se añadirán los estilos.
2. Propiedad: es el nombere del estilo CSS
3. Valor: es el valor que tomará la propiedad CSS

```css
selector {
  propiedad: valor;
}
```

## Algunas propiedades inciales

1. Color: establece el color del texto de un elemento
2. Background-color: establece un color de fondo al elemento
3. Font-size: establece el tamaño de la fuente
4. Width: establece la anchura de un elemento.
5. Height: establece la altura de un elemento

## Medidas inciales en CSS

Las medidas iniciales en CSS son las siguientes:

1. px: píxeles
2. %: establece un porcentaje con respecto a una medida base.

## Comentarios en CSS

Los comentarios en CSS consisten en señalar algo que se ignorará. Para establecer un comentario CSS se lo envuelve entre `/* y */`, independiente de la cantidad de líneas.

## Selectores de CSS

Los selectores de CSS son la forma de definir a qué elementos se les aplicará un estilo. Existen diferentes tipos de selectores, los cuales se pueden combinar entre sí para definir un estilo más específico.

**Nota:** Existen color de CSS que puedes explorar [Aqui](https://htmlcolorcodes.com/es/nombres-de-los-colores/).

### Selectores de tipo

Los selectores de tipo son aquellos que seleccionan a todos los elementos que coincidan con el nombre del selector. Por ejemplo, el selector `p` seleccionará a todos los elementos `<p>`.

### Selectores de clase

Selecciona todos los elementos que coincidan con las etiquetas HTML que contengan el atributo class

```html
<!--archivo HTML-->
<div class="card"> Soy una carta </div
```

Para seleccionar estos elementos, se empieza por un punto . Y seguido el valor exacto del atributo class de la etiqueta. Puede ser cualquier que desees colocar.

```css
/* archivo CSS */
.card {
  /* Todas las etiquetas con la clase "card" */
}
```

Pueden existir más de un valor dentro del atributo class separados por espacios.

```html
<!--archivo HTML-->
<div class="card card1">Soy una carta</div>
<div class="card card2">Soy una carta</div>
```

```css
.card {
  /* Todas las etiquetas con la clase "card" */
}

.card1 {
  /* Todas las etiquetas con la clase "card1" */
}

.card2 {
  /* Todas las etiquetas con la clase "card2" */
}
```

### Selectores de id

Selecciona el único elemento que coincida con la etiqueta HTML que contenga el atributo id. Solo puede existir un valor id para todo el documento.

```html
<!--archivo HTML-->
<button id="eliminar">Eliminar</button>
```

Para seleccionar el elemento, se empieza por el símbolo de hashtag # y seguido el valor exacto del atributo id de la etiqueta. Puede ser cualquier valor que desees colocar.

```css
/* archivo CSS */
#eliminar {
  /* La única etiqueta con el id "eliminar" */
}
```

### Selectores de atributo

Selecciona los elementos que coincidan con la etiqueta HTML que contengan el atributo y valor especificado

```html
<!--archivo HTML-->
<a href="https://platzi.com"> Ir a Platzi </a>
```

Para seleccionar los elementos, se empieza por el nombre de la etiqueta, seguido de corchetes [] que contiene el atributo y valor especificado

```css
/* archivo CSS */
a[href=""https://platzi.com"]
{
  /* Todas las etiquetas <a> con una propiedad href con valor "https://platzi.com" */
}
```

### Selectores combinados

Un selector combinador es la unión de dos o más selectores básicos

```css
Selector1 selector2 selector3 {
  /*Estilos */
}
```

### Combinador descendientes

Selecciona todos los elementos que coincidan con el selector2 que sean descendientes de selector1

```html
<!--archivo HTML-->
<div class="card">
  <h1>Soy un título</h1>
</div>
```

```css
/* archivo CSS */
.card h1 {
  /* Todos los elementos <h1> que sean descendientes de un elemento con la clase "card" */
}
```

### Combinador de hijo directo

Selecciona todos los elementos que coincidan con el selector2 que sean hijos directos de selector1

```html
<!--archivo HTML-->
<div class="card">
  <h1>Soy un título</h1>
</div>
```

```css
/* archivo CSS */
.card > h1 {
  /* Todos los elementos <h1> que sean hijos directos de un elemento con la clase "card" */
}
```

### Combinador de hermanos adyacentes

Selecciona todos los elementos que coincidan con el selector2 que sean hermanos adyacentes de selector1

```html
<!--archivo HTML-->
<div class="card">
  <h1>Soy un título</h1>
  <p>Soy un párrafo</p>
</div>
```

```css
/* archivo CSS */
h1 + p {
  /* Todos los elementos <p> que sean hermanos adyacentes de un elemento <h1> */
}
```

### Combinador de hermanos generales

Selecciona todos los elementos que coincidan con el selector2 que sean hermanos generales de selector1

```html
<!--archivo HTML-->
<div class="card">
  <h1>Soy un título</h1>
  <p>Soy un párrafo</p>
  '
  <p>Soy otro párrafo</p>
</div>
```

```css
/* archivo CSS */
h1 ~ p {
  /* Todos los elementos <p> que sean hermanos generales de un elemento <h1> */
}
```

## Pseudoclases y pseudoelementos

Existen otros tipos de selectores, además de los selectores básicos y combinadores, capaces de cambiar un estado o añadir algo más al elemento. Estos son denominados pseudoclases y pseudoelementos.

### Pseudoclases

Una pseudoclase define el estilo de un estado de un elemento.

[Documentacion](https://developer.mozilla.org/es/docs/Web/CSS/Pseudo-classes#indice_de_las_pseudo-clases_est%C3%A1ndar)

**Sintaxis**

```css
selector:pseudoclase {
  propiedad: valor;
}
```

**Algunos ejemplos de pseudoclases**

1. :hover aplica estilos cuando el cursor está sobre el elemento. [Ejemplo](https://codi.link/PGRpdj5TZcOxw6FsYW1lPC9kaXY+%7CZGl2IHsNCiAgZm9udC1zaXplOiAzcmVtOw0KICBjdXJzb3I6IHBvaW50ZXI7DQp9DQoNCmRpdjpob3ZlciB7DQogIGNvbG9yOiByZWQ7DQp9%7C)
2. :active Representa el estado de un elemento que no ha sido visitado. [Ejemplo](https://codi.link/PGEgaHJlZj0iIyI+Q2xpY2tlYW1lPC9hPg==%7CYSB7DQogIGZvbnQtc2l6ZTogM3JlbTsNCn0NCg0KYTpsaW5rIHsNCiAgY29sb3I6IHJlZDsNCn0=%7C)
3. :visited Representa el estado de un elemento que ya ha sido visitado. [Ejemplo](https://codi.link/PGEgaHJlZj0iIyI+Q2xpY2tlYW1lPC9hPg==%7CYSB7DQogIGZvbnQtc2l6ZTogM3JlbTsNCn0NCg0KYTp2aXNpdGVkIHsNCiAgY29sb3I6IHJlZDsNCn0=%7C)
4. :not Representa el estado en el cual no coinciden los selectoes que se indiquen.
   [Ejemplo](https://codi.link/PGRpdj5BenVsPC9kaXY+DQo8ZGl2PkF6dWw8L2Rpdj4NCjxkaXYgY2xhc3M9Im5lZ3JvIj5OZWdybzwvZGl2Pg0KPGRpdj5BenVsPC9kaXY+DQo8ZGl2PkF6dWw8L2Rpdj4=%7CZGl2IHsNCiAgZm9udC1zaXplOiAzcmVtOw0KfQ0KDQpkaXY6bm90KC5uZWdybykgew0KICBjb2xvcjogYmx1ZTsNCn0=%7C)
5. :ntn-child() Representa el estado en el cual coinciden los hijos del elemento segun el valor indicado.
   1. odd: los elementos hijos con posiciones impares
   2. even: los elementos hijos en posiciones pares.

[Ejemplo](https://codi.link/PGRpdj5OZWdybzwvZGl2Pg0KPGRpdj5BenVsPC9kaXY+DQo8ZGl2Pk5lZ3JvPC9kaXY+DQo8ZGl2Pk5lZ3JvPC9kaXY+DQo8ZGl2Pk5lZ3JvPC9kaXY+%7CZGl2IHsNCiAgZm9udC1zaXplOiAzcmVtOw0KfQ0KDQpkaXY6bnRoLWNoaWxkKDIpIHsNCiAgY29sb3I6IGJsdWU7DQp9%7C)

## Pseudoelementos

Un pseudoelemento define el estilo de una parte específica de un elemento.

[Documentacion](https://developer.mozilla.org/es/docs/web/css/pseudo-elements#lista_de_pseudoelementos)

**Sintaxis**

```css
selector::pseudo-elemento {
  propiedad: valor;
}
```

**Algunos pseudoelementos**

1. ::before
   Sirve para agregar un contenido antes del elemento. El contenido es agregado mediante la propiedad content de CSS.
   [Ejemplo](https://codi.link/PGgxPlTDrXR1bG88L2gxPg0KPGgyPlN1YnTDrXR1bG9zPC9oMj4NCjxoMj5TdWJ0w610dWxvczwvaDI+DQo8aDI+U3VidMOtdHVsb3M8L2gyPg0KPGgyPlN1YnTDrXR1bG9zPC9oMj4NCjxoMj5TdWJ0w610dWxvczwvaDI+DQo=%7CaDI6YmVmb3JlIHsNCiAgY29udGVudDogIiAqICI7DQogIGNvbG9yOiByZWQ7DQp9%7C)
2. ::after
   Sirve para agregar un contenido después del elemento. El contenido es agregado mediante la propiedad content de CSS.
   [Ejemplo](https://codi.link/PCEtLSBOYXZiYXIgaW1wcm92aXNhZGEgLS0+DQo8bmF2Pg0KICA8dWw+DQogICAgPGxpPkhvbWU8L2xpPg0KICAgIDxsaT5EZXN0YWNhZG9zPC9saT4NCiAgICA8bGk+RWxlbWVudG9zPC9saT4NCiAgICA8bGk+Q2xhc2VzPC9saT4NCiAgICA8bGk+TcOhcy4uLjwvbGk+DQogIDwvdWw+DQo8L25hdj4NCg==%7CbmF2IHVsIHsNCiAgbGlzdC1zdHlsZTogbm9uZTsNCiAgZGlzcGxheTogZmxleDsNCiAganVzdGlmeS1jb250ZW50OiBzcGFjZS1hcm91bmQ7DQogIGN1cnNvcjogcG9pbnRlcjsNCn0NCg0KbmF2IHVsIGxpOjphZnRlciB7DQogIGNvbnRlbnQ6ICJ8IjsNCiAgbWFyZ2luOiAxcmVtOw0KICBjb2xvcjogcmVkOw0KfQ==%7C)

3. ::first-letter
   Sirve para añadir estilos a la primera letra del texto de cualquier elemento.
   [Ejemplo](https://codi.link/PHA+U295IG90cm8gcMOhcnJhZm88L3A+DQo8cD5Tb3kgb3RybyBww6FycmFmbzwvcD4NCjxwPlNveSBvdHJvIHDDoXJyYWZvPC9wPg0KPHA+U295IG90cm8gcMOhcnJhZm88L3A+DQo8cD5Tb3kgb3RybyBww6FycmFmbzwvcD4NCjxwPlNveSBvdHJvIHDDoXJyYWZvPC9wPg0KPHA+U295IG90cm8gcMOhcnJhZm88L3A+DQo8cD5Tb3kgb3RybyBww6FycmFmbzwvcD4NCjxwPlNveSBvdHJvIHDDoXJyYWZvPC9wPg0K%7COjpmaXJzdC1sZXR0ZXJ7DQogIGNvbG9yOiByZWQ7DQp9DQo=%7C)

- [Meet the Pseudo Class Selectors | CSS-Tricks](https://css-tricks.com/pseudo-class-selectors/)
- [Pseudo-elements - CSS: Cascading Style Sheets | MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-elements)

## Cascada y especificidad en CSS

En algún punto, cuando estés creando una página web, te encontrarás con problemas con los estilos, por ejemplo:

- ¿Por qué no se aplica el color que le estoy poniendo?
- ¿Por qué este elemento se comporta de manera diferente?

Probablemente, sea un inconveniente de cascada o especificidad.

La cascada es el concepto que determina qué estilos se colocan sobre otros, priorizando a aquellos que se encuentren más abajo del código. Recordarás que CSS es la abreviación de Cascade Style Sheets, que traducido es hojas de estilos en cascada.

Mira el siguiente codigo e identifica de que color de letra tendra la etiqueta `<h1>`

```css
h1 {
  color: red;
}

h1 {
  color: blue;
}
```

La etiqueta `<h1>` tendrá un color blue de letra, esto porque está situado más abajo en el código. Esto ocurre con cada propiedad de CSS que se repite en algún punto más arriba del código.

Sin embargo, esto ocurre cuando la especificidad de una regla CSS tiene el mismo valor. Pero, ¿qué es especificidad?

La especificidad consiste en dar un valor a una regla CSS sobre qué tan específico es el estilo, esto para que los navegadores puedan saber qué estilos aplicar sobre otros, independientemente de dónde se encuentren en el código. El estilo se aplicará donde la especificidad sea mayor.

**Valor con mayor especificidad**
La palabra reservada `!important` es un valor de toda propiedad CSS que provee una especificidad de 10000, por lo que se aplicará ante otros estilos. Esto es una mala práctica y no deberías utilizarlo.

## Estilos en linea

Los estilos en línea son las propiedades CSS escritas en el HTML a través de la propiedad style de toda etiqueta. También es una mala práctica y debes evitarlo.

```html
<h1 style="color: blue">Especificad</h1>
```

## Especificidad en selectores

El tema de los selectores ya lo conoces, por lo tanto, los selectores de tipo ID son más específicos que las clases, atributos y pseudoclases. Estas últimas son más específicas que los elementos y pseudoelementos. El selector universal tiene una especificidad de 0.

En un proyecto deberías evitar los !important y estilos en línea, para trabajar únicamente con la especificidad de los selectores. Sin embargo, debes tener presente que los selectores combinadores suman la especificidad de cada selector básico para obtener la especificidad total de la regla CSS.

Si utilizas Visual Studio Code y mantienes el mouse sobre el selector, te mostrará la especificidad total. [Specificity Calculator](https://specificity.keegan.st/) es una página web donde puedes calcular la especificidad.

## Tipos de displays mas usados

La propiedad display establece el tipo de visualización de los elementos HTML sin afectar el flujo normal de los elementos.

Existen etiquetas que por defecto su display ya está determinado, como la etiqueta `<div>` que tiene display block, `<span>` tiene display inline y `<button>` tiene display inline-block.

### Block

El display block establece que un elemento ocupará todo el espacio disponible por defecto y el siguiente elemento a este se situará por debajo. Es posible añadir medidas de anchura width y altura height a estos elementos. También es posible agregar todas las propiedades del modelo de caja (no te preocupes de este concepto, ya lo abordaremos).

[Ejemplo](https://codi.link/PGRpdj5Tb3kgZGlzcGxheSBibG9jazwvZGl2Pg0KPGRpdj5Tb3kgZGlzcGxheSBibG9jazwvZGl2Pg0KPGRpdiBjbGFzcz0iY29uX21lZGlkYXMiPlNveSBkaXNwbGF5IGJsb2NrPC9kaXY+DQoNCg==%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KZGl2ew0KICBiYWNrZ3JvdW5kLWNvbG9yOiBhcXVhOw0KICAvKiBtYXJnaW46IDEwcHg7ICovDQogIC8qIHBhZGRpbmc6IDEwcHg7ICovDQp9DQoNCi5jb25fbWVkaWRhcyB7DQogIC8qIHdpZHRoOiAyMDBweDsgKi8NCiAgLyogaGVpZ2h0OiAyMDBweDsgKi8NCn0NCg0KLyogSWdub3JhIGVzdG9zIGVzdGlsb3MsIHBvciBhaG9yYSAqLw0KKiB7DQogIGZvbnQtc2l6ZTogMS4ycmVtOw0KICBtYXJnaW46IDA7DQp9DQoNCg0KDQo=%7C)

### Visualizacion en linea (inline)

El display inline establece que un elemento ocupará el espacio del contenido del mismo y el siguiente elemento se situará a la derecha. No es posible añadir medidas de anchura width y altura height a estos elementos. También, no es posible agregar todas las propiedades del modelo de caja, únicamente funcionará la propiedad margin en el eje horizontal (no te preocupes de este concepto, ya lo abordaremos).

[Ejemplo](https://codi.link/PHNwYW4+U295IGRpc3BsYXkgaW5saW5lPC9zcGFuPg0KPHNwYW4+U295IGRpc3BsYXkgaW5saW5lPC9zcGFuPg0KPHNwYW4+U295IGRpc3BsYXkgaW5saW5lPC9zcGFuPg0KPHNwYW4+U295IGRpc3BsYXkgaW5saW5lPC9zcGFuPg0KPHNwYW4gY2xhc3M9ImNvbl9tZWRpZGFzIj5Tb3kgZGlzcGxheSBpbmxpbmU8L3NwYW4+DQoNCg==%7CLyogUXVpdGEgeSBhZ3JlZ2EgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0Kc3BhbnsNCiAgYmFja2dyb3VuZC1jb2xvcjogYXF1YTsNCiAgLyogbWFyZ2luOiAyMHB4OyAqLw0KICAvKiBwYWRkaW5nOiAyMHB4OyAqLw0KfQ0KDQouY29uX21lZGlkYXMgew0KICAvKiB3aWR0aDogMjAwcHg7ICovDQogIC8qIGhlaWdodDogMjAwcHg7ICovDQp9DQoNCi8qIElnbm9yYSBlc3RvcyBlc3RpbG9zLCBwb3IgYWhvcmEgKi8NCiogew0KICBmb250LXNpemU6IDEuMnJlbTsNCiAgbWFyZ2luOiAwOw0KfQ0KDQoNCg0K%7C)

### Visualizacion de bloque y linea (inline - block)

El display inline-block combina las ventajas de bloque de colocar medidas al elemento y propiedades del modelo de caja correctamente; con las ventajas de inline de color un elemento seguido de otro en el mismo espacio.

Si algún elemento excede el contenido total, se coloca en la siguiente línea por debajo.

[Ejemplo](https://codi.link/PGJ1dHRvbj5Tb3kgZGlzcGxheSBpbmxpbmUtYmxvY2s8L2J1dHRvbj4NCjxidXR0b24+U295IGRpc3BsYXkgaW5saW5lLWJsb2NrPC9idXR0b24+DQo8YnV0dG9uPlNveSBkaXNwbGF5IGlubGluZS1ibG9jazwvYnV0dG9uPg0KPGJ1dHRvbj5Tb3kgZGlzcGxheSBpbmxpbmUtYmxvY2s8L2J1dHRvbj4NCjxidXR0b24gY2xhc3M9ImNvbl9tZWRpZGFzIj5Tb3kgZGlzcGxheSBpbmxpbmUtYmxvY2s8L2J1dHRvbj4NCg0K%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KYnV0dG9uew0KICAvKiBtYXJnaW46IDEwcHg7ICovDQogIC8qIHBhZGRpbmc6IDEwcHg7ICovDQp9DQoNCi5jb25fbWVkaWRhcyB7DQogIC8qIHdpZHRoOiAzMDBweDsgKi8NCiAgLyogaGVpZ2h0OiAxMDBweDsgKi8NCn0NCg0KLyogSWdub3JhIGVzdG9zIGVzdGlsb3MsIHBvciBhaG9yYSAqLw0KKiB7DQogIGZvbnQtc2l6ZTogMS4xcmVtOw0KICBtYXJnaW46IDA7DQp9DQoNCg0KDQo=%7C)

### Visualizacion nula (none)

El display none desactiva la visualización de un elemento, como si el elemento no existiera.

[Ejemplo](https://codi.link/PGRpdj48L2Rpdj4NCjxkaXY+PC9kaXY+DQo8ZGl2IGNsYXNzPSJkZXNhcGFyZWNlciI+DQogIEVuIG1pIHNpZ3VpZW50ZSB0cnVjbywgwqF2b3kgYSBkZXNhcGFyZWNlciENCjwvZGl2Pg0KPGRpdj48L2Rpdj4NCjxkaXY+PC9kaXY+DQo=%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KLmRlc2FwYXJlY2Vyew0KICAvKiBkaXNwbGF5OiBub25lOyAqLw0KICBiYWNrZ3JvdW5kLWNvbG9yOiBjb3JuZmxvd2VyYmx1ZTsNCiAgDQp9DQoNCi8qIElnbm9yYSBlc3RvcyBlc3RpbG9zLCBwb3IgYWhvcmEgKi8NCiogew0KICBib3gtc2l6aW5nOiBib3JkZXItYm94Ow0KICBmb250LXNpemU6IDEuMXJlbTsNCiAgbWFyZ2luOiAwOw0KfQ0KDQpib2R5ew0KICBkaXNwbGF5OiBmbGV4Ow0KfQ0KDQpkaXZ7DQogIGJhY2tncm91bmQtY29sb3I6IGNvcmFsOw0KICB3aWR0aDogMTIwcHg7DQogIGhlaWdodDogMTIwcHg7DQogIGZvbnQtd2VpZ2h0OiA4MDA7DQogIHBhZGRpbmc6IDhweDsNCn0NCg0KDQoNCg==%7C)

## Flexbox y CSS Grid

El display flex y grid son formas de visualización de elementos recientes y cada uno tienen sus propias características para crear interfaces de manera efectiva, a partir de un contenedor padre que dotará a los elementos hijos de superpoderes del posicionamiento.

Ambas son herramientas muy útiles en el desarrollo, especialmente para la creación de interfaces amigables al usuario y aptas para cualquier dispositivo, que a este último se lo conoce como responsive design.

### Flexbox

Flexbox consiste en el ordenamiento de elementos hijos en un solo eje, por defecto horizontalmente. El elemento padre o contenedor deberá contener la propiedad display con el valor flex. A partir de aquí, ya puedes ordenar los hijos según sea necesario.

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCjwvZGl2Pg0KDQoNCg0K%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCn0NCg0KLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KLmNvbnRhaW5lcnsNCiAgLyogZGlzcGxheTogZmxleDsgKi8NCn0NCg0KLmNvbnRhaW5lciBkaXYgew0KICB3aWR0aDogMTAwcHg7IA0KICBoZWlnaHQ6IDEwMHB4Ow0KfQ0KDQouY29udGFpbmVyIGRpdjpudGgtY2hpbGQoMm4pew0KICBiYWNrZ3JvdW5kLWNvbG9yOiBhcXVhOw0KfQ0KDQouY29udGFpbmVyIGRpdjpudGgtY2hpbGQoMm4rMSl7DQogIGJhY2tncm91bmQtY29sb3I6IGJyb3duOw0KfQ0KDQoNCg0KDQoNCg0K%7C)

### Grid

Grid consiste en el ordenamiento de elementos hijos en dos ejes, como si fuera una cuadrícula o tabla. El elemento padre o contenedor deberá contener la propiedad display con el valor grid y debes definir las medidas de las columnas y de las filas. A partir de aquí, ya puedes ordenar los hijos según sea necesario.

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCiAgPGRpdj48L2Rpdj4NCjwvZGl2Pg0KDQoNCg0K%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCn0NCg0KLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KLmNvbnRhaW5lcnsNCi8qICAgDQogIGRpc3BsYXk6IGdyaWQ7DQogIGdyaWQtdGVtcGxhdGUtY29sdW1uczogMTAwcHggMTAwcHggMTAwcHg7DQogIGdyaWQtdGVtcGxhdGUtcm93czogMTAwcHggMTAwcHggMTAwcHg7IA0KICAqLw0KDQoNCn0NCg0KLmNvbnRhaW5lciBkaXYgew0KICB3aWR0aDogMTAwcHg7IA0KICBoZWlnaHQ6IDEwMHB4Ow0KfQ0KDQouY29udGFpbmVyIGRpdjpudGgtY2hpbGQoMm4pew0KICBiYWNrZ3JvdW5kLWNvbG9yOiBhcXVhOw0KfQ0KDQouY29udGFpbmVyIGRpdjpudGgtY2hpbGQoMm4rMSl7DQogIGJhY2tncm91bmQtY29sb3I6IGJyb3duOw0KfQ0KDQoNCg0KDQoNCg0K%7C)

- [Flexbox vs CSS Grid: ¿Cuál es la diferencia?](https://platzi.com/blog/flexbox-vs-css-grid-cual-es-la-diferencia/)
- [A Complete Guide to Flexbox](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

## Modelo de caja

El modelo de caja se compone de cuatro elementos: margin, border, padding y contenido.
Si entras a las herramientas de desarrollador de tu navegador y señalas un elemento HTML, en la sección de estilos te aparecerá una vista parecida a la anterior imagen, este es el modelo de caja del elemento señalado.

![02](https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.eniun.com%2Fmodelo-cajas-css-margenes-relleno-bordes%2F&psig=AOvVaw260h1zxZTeqWsovw3Lxa0n&ust=1690659041252000&source=images&cd=vfe&opi=89978449&ved=0CBEQjRxqFwoTCJCwye6RsoADFQAAAAAdAAAAABAI)

## Content

El contenido del elemento, como su nombre lo indica, es todo lo que está dentro del elemento. Este tiene medidas establecidas por las propiedades width y height, que representan la anchura y la altura, respectivamente. Si imaginamos una caja, este valor sería todo lo que decidas colocar dentro.

## Border

El border consiste en el perfil o borde de un elemento HTML. Si imaginamos una caja, sería la caja en sí. Para definir un borde es necesario utilizar las siguientes tres propiedades:

- border-color: establece el color del borde.
- border-style: establece el estilo propio del borde, estos pueden ser: none (sin borde), dotted (puntos), dashed (guiones), solid (continuo), double (doble continuo), groove (recuadro).
- border-width: estable la anchura del borde.

También se puede establecer los tres valores en una sola propiedad border donde no importa el orden.

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0ibm9uZSI+U2luIGJvcmRlPC9kaXY+DQo8ZGl2IGNsYXNzPSJkb3R0ZWQiPkNvbiBwdW50b3M8L2Rpdj4NCjxkaXYgY2xhc3M9ImRhc2hlZCI+Q29uIGd1aW9uZXM8L2Rpdj4NCjxkaXYgY2xhc3M9InNvbGlkIj5Db250aW51bzwvZGl2Pg0KPGRpdiBjbGFzcz0iZG91YmxlIj5kb2JsZSBjb250aW51bzwvZGl2Pg0KPGRpdiBjbGFzcz0iZ3Jvb3ZlIj5Db24gcmVjdWFkcm88L2Rpdj4NCg0KDQo=%7CZGl2ew0KICB3aWR0aDogMTIwcHg7DQogIGhlaWdodDogMTIwcHg7DQp9DQoNCi5ub25lew0KICAvKiBWYWxvciBwb3IgZGVmZWN0byBkZSBkaXYgKi8NCiAgYm9yZGVyOiAzcHggYmxhY2sgbm9uZTsNCn0NCg0KLmRvdHRlZHsNCiAgYm9yZGVyOiAzcHggYmxhY2sgZG90dGVkOw0KfQ0KDQouZGFzaGVkew0KICBib3JkZXI6IDNweCBibGFjayBkYXNoZWQ7DQp9DQoNCi5zb2xpZHsNCiAgYm9yZGVyOiAzcHggYmxhY2sgc29saWQ7DQp9DQoNCi5kb3VibGV7DQogIGJvcmRlcjogM3B4IGJsYWNrIGRvdWJsZTsNCn0NCg0KLmdyb292ZXsNCiAgYm9yZGVyOiA1cHggZ3JlZW55ZWxsb3cgZ3Jvb3ZlOw0KfQ0KDQoNCg0KLyogSWdub3JhIGVzdG9zIGVzdGlsb3MsIHBvciBhaG9yYSAqLw0KKiB7DQogIGZvbnQtc2l6ZTogMS4xcmVtOw0KICBtYXJnaW46IDA7DQp9DQoNCmJvZHl7DQogIGRpc3BsYXk6IGZsZXg7DQogIGZsZXgtd3JhcDogd3JhcDsNCiAgZ2FwOiAxLjVyZW07DQogIG1hcmdpbjogMjBweDsNCiAgZm9udC13ZWlnaHQ6IDgwMDsNCn0NCg0KDQoNCg==%7C)

```css
div {
  border: [color] [style] [width];
}

div {
  border-color: red;
  border-style: solid;
  border-width: 1px;
}
```

También estableciendo de manera individual los valores de cada posición:

```css
div {
    border-top: 5px solid blue;
    border-bottom: 5px solid red;
    border-left: 5px solid black
    border-right: 5px solid yellow;
}
```

## Padding

El padding consiste en el espacio entre el borde y el contenido del elemento HTML. Si imaginamos una caja, este valor sería el espacio entre la caja y lo que deseas guardar.

[Ejemplo](https://codi.link/PGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KDQoNCg==%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KZGl2ew0KICB3aWR0aDogMTIwcHg7DQogIGhlaWdodDogMTIwcHg7DQogIGJhY2tncm91bmQtY29sb3I6IGdyZWVueWVsbG93Ow0KICBib3JkZXI6IHNvbGlkIDFweCBibGFjazsNCiAgLyogcGFkZGluZzogMzBweDsgKi8NCn0NCg0KDQoNCi8qIElnbm9yYSBlc3RvcyBlc3RpbG9zLCBwb3IgYWhvcmEgKi8NCiogew0KICBmb250LXNpemU6IDEuMXJlbTsNCiAgbWFyZ2luOiAwLjVyZW07DQp9DQo=%7C)

Puedes establecer el padding en cada posicion en una sola linea de las siguientes maneras:

- padding: [arriba] [derecha] [abajo] [izquierda], siguiendo el sentido horario.
- padding: [arriba] [abajo] [derecha e izquierda], siguiendo el eje principal.
- padding: [arriba y abajo] [derecha e izquierda], siguiendo los ejes del elemento.

También estableciendo de manera individual los valores de cada posición:

```css
div {
  padding-top: 10px;
  padding-bottom: 15px;
  padding-left: 20px;
  padding-right: 10px;
}
```

## Margin

El margin consiste en el espacio entre el borde y otro elemento HTML. Si imaginamos una caja, es el espacio entre tu caja y otra caja

```css
div {
  margin-top: 10px;
  margin-bottom: 15px;
  margin-left: 20px;
  margin-right: 10px;
}
```

## Valores por defecto

Por defecto, el navegador establece valores iniciales a algunas propiedades CSS, este es el caso de margin y padding. Una buena práctica es utilizar el selector universal para restablecer estos valores a 0, para que no surjan errores inesperados.

## El tamanio total del elemento

El tamaño total del elemento está determinado por la suma de los valores de las propiedades border padding y width o height, dependiendo del eje. La propiedad margin no está incluida en este cálculo

Por ejemplo, definimos los siguientes estilos:

```css
div {
  width: 150px;
  height: 150px;
  padding: 20px;
  border: 10px solid gray;
  margin: 30px;
}
```

El tamaño total del elemento será de 210px en ambos ejes, donde la suma fue: 150 (altura/anchura) + 20 x 2 (padding ambos lados) + 10 x 2 (borde ambos lados). Si evaluamos este elemento en las herramientas del desarrollador mostrará su tamaño como 210x210.

Aunque se conozcan las medidas de los elementos de esta manera, no siempre existirá un control total. Por lo que podríamos establecer el tamaño total del elemento con width y height, y no solo del contenido, añadiendo la propiedad box-sizing.

## Propiedad box-sizing

La propiedad box-sizing establece cómo se calculará el width y el height sí incluyen bordes y espacios internos. Como buena práctica, se lo coloca en el selector universal, para que todos los elementos sigan esta tendencia.

Con el valor border-box, el tamaño total del elemento será igual al especificado en el width y height, provocando que las medidas del contenido cambien con respecto a los bordes y espacios internos.

[Ejemplo](https://codi.link/PGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KDQoNCg==%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBsbyBxdWUgb2N1cnJlICovDQoqIHsNCiAgbWFyZ2luOiAwOw0KICBwYWRkaW5nOiAwOw0KICAvKiBib3gtc2l6aW5nOiBib3JkZXItYm94OyAqLw0KfQ0KDQpkaXZ7DQogIGJhY2tncm91bmQtY29sb3I6IGdyZWVueWVsbG93Ow0KICB3aWR0aDogMTUwcHg7DQogIGhlaWdodDogMTUwcHg7DQogIHBhZGRpbmc6IDIwcHg7DQogIGJvcmRlcjogMTBweCBzb2xpZCBncmF5Ow0KICBtYXJnaW46IDMwcHg7DQp9DQoNCg0KDQoNCg0K%7C)

El tamaño total del elemento será de 150px en ambos ejes, donde se calcularon las medidas del contenido para que la suma total sea lo especificado en el width y height. Si evaluamos este elemento en las herramientas del desarrollador mostrará su tamaño total como 150x150 y el contenido como 90x90.

Conclusión, establece las medidas totales del elemento con width y height, junto con box-sizing: border-box, para que el contenido se adecue a las necesidades del contenedor.

### Problema con el tamaño de los bordes

Recapitulando, el tamaño total de un elemento es la suma de tres: el borde, el espacio interior y el contenido.

Entonces, en algunas ocasiones tendrás la intención de añadir un borde al realizar un hover. Esto provocará que el elemento necesite más espacio del inicial, en un contenedor con más elementos puede ocasionar un conflicto.

Mira el siguiente ejemplo, e intenta poner el cursor sobre un elemento ¿qué sucede?

[Ejemplo](https://codi.link/PGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KPGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KDQoNCg==%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBsbyBxdWUgb2N1cnJlICovDQoqIHsNCiAgbWFyZ2luOiAwOw0KICBwYWRkaW5nOiAwOw0KfQ0KDQpkaXZ7DQogIGRpc3BsYXk6IGlubGluZS1ibG9jazsNCiAgYmFja2dyb3VuZC1jb2xvcjogZ3JlZW55ZWxsb3c7DQogIHdpZHRoOiAxNTBweDsNCiAgaGVpZ2h0OiAxNTBweDsNCiAgcGFkZGluZzogMjBweDsNCiAgbWFyZ2luOiAzMHB4Ow0KfQ0KDQpkaXY6aG92ZXJ7DQogIGJvcmRlcjogMTBweCBzb2xpZCBncmF5Ow0KICBjdXJzb3I6IHBvaW50ZXI7DQp9DQoNCg0KDQoNCg0K%7C)

Observaste este comportamiento, debes tener cuidado con lo que agregas porque puedes provocar errores.

La solución a esto es colocar un borde de color transparent (transparente) y del mismo tamaño que el otro borde. Esto hará que el elemento se mantenga en su tamaño total, lo único que cambia es el color.

[Ejemplo](https://codi.link/PGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KPGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KDQoNCg==%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBsbyBxdWUgb2N1cnJlICovDQoqIHsNCiAgbWFyZ2luOiAwOw0KICBwYWRkaW5nOiAwOw0KfQ0KDQpkaXZ7DQogIGRpc3BsYXk6IGlubGluZS1ibG9jazsNCiAgYmFja2dyb3VuZC1jb2xvcjogZ3JlZW55ZWxsb3c7DQogIHdpZHRoOiAxNTBweDsNCiAgaGVpZ2h0OiAxNTBweDsNCiAgcGFkZGluZzogMjBweDsNCiAgbWFyZ2luOiAzMHB4Ow0KICAvKiBib3JkZXI6IDEwcHggc29saWQgdHJhbnNwYXJlbnQ7ICovDQp9DQoNCmRpdjpob3ZlcnsNCiAgYm9yZGVyOiAxMHB4IHNvbGlkIGdyYXk7DQogIGN1cnNvcjogcG9pbnRlcjsNCn0NCg0KDQoNCg0KDQo=%7C)

Evita agregar un tamaño diferente al inicial.

## Colapso de margenes

El colapso de márgenes sucede cuando dos elementos bloque adyacentes tienen un determinado valor de margin, entonces estos márgenes se solapan en un solo valor, el mayor de ambos.

![03](https://static.platzi.com/media/articlases/Images/frontend_developer25.png)

[Ejemplo](https://codi.link/PGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KPGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KPGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KPGRpdj5Mb3JlbSBpcHN1bSBkb2xvciBzaXQgYW1ldCBjb25zZWN0ZXR1ciBhZGlwaXNpY2luZyBlbGl0aTwvZGl2Pg0KDQoNCg0K%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCn0NCg0KLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBsbyBxdWUgb2N1cnJlICovDQpkaXZ7DQogIC8qIGRpc3BsYXk6IGlubGluZS1ibG9jazsgKi8NCiAgbWFyZ2luOiA0MHB4Ow0KICBiYWNrZ3JvdW5kLWNvbG9yOiBncmVlbnllbGxvdzsNCiAgd2lkdGg6IDgwJTsNCiAgaGVpZ2h0OiA1MHB4Ow0KICBwYWRkaW5nOiAxMHB4Ow0KfQ0KDQoNCg0KDQoNCg0K%7C)

Al cambiar el display este comportamiento desaparece. Además, en flexbox y grid no ocurre el colapso de márgenes. Cuida los márgenes que colocas en los elementos de tipo bloque.

## Posicionamiento en CSS

El posicionamiento en CSS consiste en cómo un elemento se situará, con respecto a su elemento padre y al flujo normal del documento. El flujo normal del documento es el orden de los elementos establecidos en el HTML.

La posición del elemento se la define con la propiedad position, mediante los siguientes valores:

1. static
2. relative
3. absolute
4. sticky

### Propiedades de posicion

Además de la propiedad position, existen cuatro propiedades del elemento de acuerdo a su posición con respecto a su padre, estas son: top (arriba), bottom (debajo), left (izquierda) y right (derecha).

```css
div {
  top: 10px;
  bottom: 15px;
  left: 20px;
  rigth: 10px;
}
```

Estos valores están establecidos en el padre próximo que tenga la posición relative. Si top y bottom están definidos, top gana. Si left y rigth están definidos, left gana (dependiendo el idioma configurado).

1. **Posicion estatica:** La posición static es el valor por defecto de todo elemento HTML, consiste en respetar el flujo normal del documento donde las propiedades de posición no pueden ser establecidas.
2. **Posicion relative:** La posición relative consiste en respetar el flujo normal del documento donde las propiedades de posición sí pueden ser establecidas.
   [Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdiBjbGFzcz0icmVsYXRpdmUiPjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KICA8ZGl2PjwvZGl2Pg0KPC9kaXY+DQoNCg0KDQo=%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCn0NCg0KLmNvbnRhaW5lcnsNCiAgd2lkdGg6IDEwMCU7DQp9DQoNCi5jb250YWluZXIgZGl2IHsNCiAgd2lkdGg6IDEwMHB4OyANCiAgaGVpZ2h0OiAxMDBweDsNCn0NCg0KLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KLmNvbnRhaW5lciAucmVsYXRpdmV7DQogIC8qIHBvc2l0aW9uOiByZWxhdGl2ZTsgKi8NCiAgLyogdG9wOiA1MHB4OyAqLw0KICAvKiBsZWZ0OiA1MHB4OyAqLw0KfQ0KDQouY29udGFpbmVyIGRpdjpudGgtY2hpbGQoMm4pew0KICBiYWNrZ3JvdW5kLWNvbG9yOiBhcXVhOw0KfQ0KDQouY29udGFpbmVyIGRpdjpudGgtY2hpbGQoMm4rMSl7DQogIGJhY2tncm91bmQtY29sb3I6IGJyb3duOw0KfQ0KDQoNCg0KDQoNCg0K%7C)
3. **Posicion absoluta:** La posición absolute consiste en quitar al elemento del flujo normal del documento donde las propiedades de posición sí pueden ser establecidas.
   [Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY29udGFpbmVyIj4NCiAgPGRpdiBjbGFzcz0iYWJzb2x1dGUiPjE8L2Rpdj4NCiAgPGRpdj4yPC9kaXY+DQogIDxkaXY+MzwvZGl2Pg0KICA8ZGl2PjQ8L2Rpdj4NCiAgPGRpdj41PC9kaXY+DQo8L2Rpdj4NCg0KDQoNCg==%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCiAgZm9udC1zaXplOiAxLjVyZW07DQp9DQoNCi8qIEltcG9ydGFudGUgZWwgcG9zaXRpb24gKi8NCi5jb250YWluZXJ7DQogIHBvc2l0aW9uOiByZWxhdGl2ZTsNCiAgd2lkdGg6IDEwMCU7DQp9DQoNCi5jb250YWluZXIgZGl2IHsNCiAgd2lkdGg6IDEwMHB4OyANCiAgaGVpZ2h0OiAxMDBweDsNCn0NCg0KLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KLmNvbnRhaW5lciAuYWJzb2x1dGV7DQogIC8qIHBvc2l0aW9uOiBhYnNvbHV0ZTsgKi8NCiAgLyogbGVmdDogMTUwcHg7ICovDQogIC8qIHRvcDogNTBweDsgKi8NCn0NCg0KLmNvbnRhaW5lciBkaXY6bnRoLWNoaWxkKDJuKXsNCiAgYmFja2dyb3VuZC1jb2xvcjogYXF1YTsNCn0NCg0KLmNvbnRhaW5lciBkaXY6bnRoLWNoaWxkKDJuKzEpew0KICBiYWNrZ3JvdW5kLWNvbG9yOiBicm93bjsNCn0NCg0KDQoNCg0KDQoNCg0KDQo=%7C)

Habrás notado que el elemento “2” desaparece, pero en realidad lo que sucede es que se sitúa por detrás del elemento con posición absoluta que salió del flujo normal del documento. Este comportamiento se debe al eje Z de la pantalla y al contexto de apilamiento.

El elemento con posición absoluta se desplazará arriba, abajo, izquierda o derecha con respecto al elemento padre más próximo con posición relativa.

Si no existe un padre con posición relativa de un elemento con posición absoluta, este se desplazará con respecto al elemento raíz del documento.

En el siguiente ejemplo, te encontrarás varios contenedores padres, incluso las etiquetas `<html> y <body>`. Sigue los pasos y observa el comportamiento. Ignora los estilos iniciales, simplemente sirven para establecer la estructura del ejercicio.

[Ejemplo](https://codi.link/PHA+Qm9keTwvcD4NCjxkaXYgY2xhc3M9ImFidWVsbyI+DQogIDxwPkFidWVsbzwvcD4NCiAgPGRpdiBjbGFzcz0icGFkcmUiPg0KICAgIDxwPlBhZHJlPC9wPg0KICAgIDxkaXYgY2xhc3M9Imhpam8iPg0KICAgICAgPHA+SGlqbzwvcD4NCiAgICA8L2Rpdj4NCiAgPC9kaXY+DQo8L2Rpdj4=%7CLyogRWwgZWplcmNpY2lvIGVzdMOhIGhhc3RhIGFiYWpvICovDQoNCiogew0KICBtYXJnaW46IDA7DQogIHBhZGRpbmc6IDA7DQogIGJveC1zaXppbmc6IGJvcmRlci1ib3g7DQogIHRleHQtYWxpZ246IGNlbnRlcjsNCn0NCg0KaHRtbHsNCiAgbWFyZ2luOiAyMHB4Ow0KICBib3JkZXI6IDFweCByZWQgc29saWQ7DQp9DQoNCmJvZHkgew0KICBtYXJnaW46IDIwcHg7DQogIGJhY2tncm91bmQtY29sb3I6IHdoZWF0Ow0KICBib3JkZXI6IDFweCBibGFjayBzb2xpZDsNCn0NCg0KcCB7DQogIGZvbnQtc2l6ZTogMS41cmVtOw0KICBmb250LXdlaWdodDogYm9sZDsNCiAgbWFyZ2luLWJvdHRvbTogNTBweDsNCg0KfQ0KDQouYWJ1ZWxvew0KICB3aWR0aDogMTAwJTsNCiAgaGVpZ2h0OiAxMDB2aDsNCiAgYmFja2dyb3VuZC1jb2xvcjogeWVsbG93Z3JlZW47DQp9DQoNCi5wYWRyZXsNCiAgd2lkdGg6IDc1JTsNCiAgaGVpZ2h0OiA3NSU7DQogIGJhY2tncm91bmQtY29sb3I6IGNhZGV0Ymx1ZTsNCn0NCg0KLmhpam97DQogIHdpZHRoOiAxNTBweDsNCiAgaGVpZ2h0OiAxNTBweDsNCiAgYmFja2dyb3VuZC1jb2xvcjogcm9zeWJyb3duOyANCn0NCg0KDQovKiBMbyDDum5pY28gcXVlIHF1aWVybyBxdWUgZW50aWVuZGFzIGVzIHF1ZSBoYXkgMyBjb250ZW5lZG9yZXMsIGxvcyBjdcOhbGVzIA0KLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCBjb21wb3J0YW1pZW50byAqLw0KDQoNCi5oaWpvIHsNCiAgLyogcG9zaXRpb246IGFic29sdXRlOyAqLw0KICAvKiB0b3A6IDA7ICovDQp9DQoNCi8qIMK/IFBvciBxdcOpIHN1Y2VkacOzIGVzdG8gPyAqLw0KDQpodG1sIHsNCiAgLyogcG9zaXRpb246IHJlbGF0aXZlOyAqLw0KfQ0KDQpib2R5IHsNCiAgLyogcG9zaXRpb246IHJlbGF0aXZlOyAqLw0KfQ0KDQouYWJ1ZWxvew0KICAvKiBwb3NpdGlvbjogcmVsYXRpdmU7ICovDQp9DQoNCi5wYWRyZSB7DQogIC8qIHBvc2l0aW9uOiByZWxhdGl2ZTsgKi8NCn0NCg0KLyogwr8gQWhvcmEgZW50ZW5kaXN0ZSA/ICovDQoNCg0KDQoNCg0KDQoNCg0K%7C)

Como pudiste observar, en el elemento con posición absoluta, su desplazamiento se basa con relación al elemento padre más próximo con posición relativa.

## Posicion fija

La posición fixed consiste en quitar al elemento del flujo normal del documento y fijarlo en un lugar; donde las propiedades de posición sí pueden ser establecidas.En el siguiente ejemplo, desplázate por el documento, observa el comportamiento antes y después de colocar la posición fija.

[Ejemplo](https://codi.link/PG5hdj5EZSBncmFuZGUgcXVpZXJvIHNlciB1bmEgYmFycmEgZGUgbmF2ZWdhY2nDs248L25hdj4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQo8cD5Tb3kgdW4gcMOhcnJhZm8sIGJhamEgcG9yIGZhdm9yPC9wPg0KPHA+U295IHVuIHDDoXJyYWZvLCBiYWphIHBvciBmYXZvcjwvcD4NCjxwPlNveSB1biBww6FycmFmbywgYmFqYSBwb3IgZmF2b3I8L3A+DQoNCg0KDQo=%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCiAgZm9udC1zaXplOiAxLjFyZW07DQp9DQoNCi8qIERlc3Bsw6F6YXRlIHBvciBlbCBkb2N1bWVudG8geSBkZXNwdcOpcyBxdWl0YSBsb3MgY29tZW50YXJpb3MgeSBvYnNlcnZhIGVsIGNvbXBvcnRhbWllbnRvICovDQoNCm5hdiB7DQogIC8qIHBvc2l0aW9uOiBmaXhlZDsgKi8NCiAgLyogdG9wOiAwOyAqLw0KICBiYWNrZ3JvdW5kLWNvbG9yOiBjb3JuZmxvd2VyYmx1ZTsNCiAgd2lkdGg6IDEwMCU7DQogIGhlaWdodDogYXV0bzsNCiAgcGFkZGluZzogMjBweDsNCn0NCg0KcCB7DQogIHBhZGRpbmc6IDEwcHg7DQp9DQoNCg0KDQoNCg0KDQoNCg0K%7C)

## Posicion variable fija

La posición sticky consiste en quitar al elemento del flujo normal del documento y fijarlo en un lugar mientras su contenedor sea visible; donde las propiedades de posición sí pueden ser establecidas.

En el siguiente ejemplo, desplázate por el documento, observa el comportamiento antes y después de colocar la posición variable fija.

[Ejemplo](https://codi.link/PGRpdj4NCiAgPHA+U295IHVuIHDDoXJyYWZvIDE8L3A+DQogIDx1bD4NCiAgICA8bGk+RWxlbWVudG8gMTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDI8L2xpPg0KICAgIDxsaT5FbGVtZW50byAzPC9saT4NCiAgICA8bGk+RWxlbWVudG8gNDwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDU8L2xpPg0KICAgIDxsaT5FbGVtZW50byA2PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDg8L2xpPg0KICAgIDxsaT5FbGVtZW50byA5PC9saT4NCiAgICA8bGk+RWxlbWVudG8gMTA8L2xpPg0KICA8L3VsPg0KICA8cD5Tb3kgdW4gcMOhcnJhZm8gMjwvcD4NCiAgPHVsPg0KICAgIDxsaT5FbGVtZW50byAxPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDM8L2xpPg0KICAgIDxsaT5FbGVtZW50byA0PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDY8L2xpPg0KICAgIDxsaT5FbGVtZW50byA3PC9saT4NCiAgICA8bGk+RWxlbWVudG8gODwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDk8L2xpPg0KICAgIDxsaT5FbGVtZW50byAxMDwvbGk+DQogIDwvdWw+DQogIDxwPlNveSB1biBww6FycmFmbyAzPC9wPg0KICA8dWw+DQogICAgPGxpPkVsZW1lbnRvIDE8L2xpPg0KICAgIDxsaT5FbGVtZW50byAyPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDQ8L2xpPg0KICAgIDxsaT5FbGVtZW50byA1PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDc8L2xpPg0KICAgIDxsaT5FbGVtZW50byA4PC9saT4NCiAgICA8bGk+RWxlbWVudG8gOTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDEwPC9saT4NCiAgPC91bD4NCiAgPHA+U295IHVuIHDDoXJyYWZvIDQ8L3A+DQogIDx1bD4NCiAgICA8bGk+RWxlbWVudG8gMTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDI8L2xpPg0KICAgIDxsaT5FbGVtZW50byAzPC9saT4NCiAgICA8bGk+RWxlbWVudG8gNDwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDU8L2xpPg0KICAgIDxsaT5FbGVtZW50byA2PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDg8L2xpPg0KICAgIDxsaT5FbGVtZW50byA5PC9saT4NCiAgICA8bGk+RWxlbWVudG8gMTA8L2xpPg0KICA8L3VsPg0KICA8cD5Tb3kgdW4gcMOhcnJhZm8gNTwvcD4NCiAgPHVsPg0KICAgIDxsaT5FbGVtZW50byAxPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDM8L2xpPg0KICAgIDxsaT5FbGVtZW50byA0PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDY8L2xpPg0KICAgIDxsaT5FbGVtZW50byA3PC9saT4NCiAgICA8bGk+RWxlbWVudG8gODwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDk8L2xpPg0KICAgIDxsaT5FbGVtZW50byAxMDwvbGk+DQogIDwvdWw+DQogIDxwPlNveSB1biBww6FycmFmbyA2PC9wPg0KICA8dWw+DQogICAgPGxpPkVsZW1lbnRvIDE8L2xpPg0KICAgIDxsaT5FbGVtZW50byAyPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDQ8L2xpPg0KICAgIDxsaT5FbGVtZW50byA1PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDc8L2xpPg0KICAgIDxsaT5FbGVtZW50byA4PC9saT4NCiAgICA8bGk+RWxlbWVudG8gOTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDEwPC9saT4NCiAgPC91bD4NCiAgPHA+U295IHVuIHDDoXJyYWZvIDc8L3A+DQogIDx1bD4NCiAgICA8bGk+RWxlbWVudG8gMTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDI8L2xpPg0KICAgIDxsaT5FbGVtZW50byAzPC9saT4NCiAgICA8bGk+RWxlbWVudG8gNDwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDU8L2xpPg0KICAgIDxsaT5FbGVtZW50byA2PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDg8L2xpPg0KICAgIDxsaT5FbGVtZW50byA5PC9saT4NCiAgICA8bGk+RWxlbWVudG8gMTA8L2xpPg0KICA8L3VsPg0KICA8cD5Tb3kgdW4gcMOhcnJhZm8gODwvcD4NCiAgPHVsPg0KICAgIDxsaT5FbGVtZW50byAxPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDM8L2xpPg0KICAgIDxsaT5FbGVtZW50byA0PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDY8L2xpPg0KICAgIDxsaT5FbGVtZW50byA3PC9saT4NCiAgICA8bGk+RWxlbWVudG8gODwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDk8L2xpPg0KICAgIDxsaT5FbGVtZW50byAxMDwvbGk+DQogIDwvdWw+DQogIDxwPlNveSB1biBww6FycmFmbyA5PC9wPg0KICA8dWw+DQogICAgPGxpPkVsZW1lbnRvIDE8L2xpPg0KICAgIDxsaT5FbGVtZW50byAyPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDQ8L2xpPg0KICAgIDxsaT5FbGVtZW50byA1PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDc8L2xpPg0KICAgIDxsaT5FbGVtZW50byA4PC9saT4NCiAgICA8bGk+RWxlbWVudG8gOTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDEwPC9saT4NCiAgPC91bD4NCiAgPHA+U295IHVuIHDDoXJyYWZvIDEwPC9wPg0KICA8dWw+DQogICAgPGxpPkVsZW1lbnRvIDE8L2xpPg0KICAgIDxsaT5FbGVtZW50byAyPC9saT4NCiAgICA8bGk+RWxlbWVudG8gMzwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDQ8L2xpPg0KICAgIDxsaT5FbGVtZW50byA1PC9saT4NCiAgICA8bGk+RWxlbWVudG8gNjwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDc8L2xpPg0KICAgIDxsaT5FbGVtZW50byA4PC9saT4NCiAgICA8bGk+RWxlbWVudG8gOTwvbGk+DQogICAgPGxpPkVsZW1lbnRvIDEwPC9saT4NCiAgPC91bD4NCjwvZGl2Pg==%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCiAgZm9udC1zaXplOiAxLjFyZW07DQp9DQoNCi8qIERlc3Bsw6F6YXRlIHBvciBlbCBkb2N1bWVudG8geSBkZXNwdcOpcyBxdWl0YSBsb3MgY29tZW50YXJpb3MgeSBvYnNlcnZhIGVsIGNvbXBvcnRhbWllbnRvICovDQoNCnAgew0KICAvKiBwb3NpdGlvbjogc3RpY2t5OyAqLw0KICAvKiB0b3A6IDA7ICovDQogIGJhY2tncm91bmQtY29sb3I6IGNvcm5mbG93ZXJibHVlOw0KICBwYWRkaW5nOiAxMHB4Ow0KfQ0KDQpsaSB7DQogIG1hcmdpbjogMjBweCAzMHB4Ow0KfQ0KDQoNCg0KDQoNCg0KDQoNCg0K%7C)

## Z - index y el contexto de apilamiento

El contexto de apilamiento consiste en la superposición de capas o elementos a lo largo del eje Z del navegador. Esto es importante para evitar que un elemento esté ocultando a otro.

El contexto de apilamiento se configura con la propiedad z-index.

Por defecto, todos los elementos tienen un valor auto, es decir, el orden está definido por la estructura del HTML. Los primeros elementos estarán detrás y los últimos estarán de frente.

Si se establece un valor positivo, este elemento se sitúa por delante de los demás. Si se establece un valor negativo, se sitúa por detrás.

Si un elemento tiene un z-index mayor a otro, estará por delante. Sin embargo, si un elemento que tiene un z-index menor a otros, sus hijos nunca estarán por encima, aunque su z-index sea mayor.

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0icmVkIj5SZWQ8L2Rpdj4NCjxkaXYgY2xhc3M9ImJsdWUiPkJsdWUNCiAgPGRpdiBjbGFzcz0ieWVsbG93Ij4NCiAgICBZZWxsb3cgKGhpam8gZGUgYmx1ZSkNCiAgPC9kaXY+DQo8L2Rpdj4=%7CLyogUXVpdGEgbG9zIGNvbWVudGFyaW9zIHkgb2JzZXJ2YSBlbCByZXN1bHRhZG8gKi8NCg0KZGl2IHsNCiAgLyogcG9zaXRpb246IGFic29sdXRlOyAqLw0KfQ0KDQoucmVkew0KICAvKiB6LWluZGV4OiA1OyAqLw0KICAvKiB0b3A6IDUwcHg7ICovDQp9DQoNCi5ibHVlew0KICAvKiB6LWluZGV4OiA0OyAqLw0KICAvKiBsZWZ0OiA1MHB4OyAqLw0KfQ0KDQoueWVsbG93ew0KICAvKiB6LWluZGV4OiA2OyAqLw0KICAvKiByaWdodDogLTIwcHg7ICovDQogIC8qIHRvcDogNDBweDsgKi8NCn0NCg0KDQovKiBJZ25vcmEgbG9zIHNpZ3VpZW50ZXMgZXN0aWxvcyAqLw0KDQoqIHsNCiAgbWFyZ2luOiAwOw0KICBwYWRkaW5nOiAwOw0KICBib3gtc2l6aW5nOiBib3JkZXItYm94Ow0KICBmb250LXNpemU6IDEuMXJlbTsNCn0NCg0KZGl2IHsNCiAgd2lkdGg6IDIwMHB4Ow0KICBoZWlnaHQ6IDIwMHB4Ow0KfQ0KDQoucmVkew0KICBiYWNrZ3JvdW5kLWNvbG9yOiByZ2IoMjQ2LCAxMDgsIDEwOCk7DQp9DQoNCi5ibHVlew0KICBiYWNrZ3JvdW5kLWNvbG9yOiByZ2IoMTAyLCAxMDIsIDI0OSk7DQp9DQoNCi55ZWxsb3d7DQogIHdpZHRoOiAxNTBweDsNCiAgaGVpZ2h0OiAxNTBweDsNCiAgYmFja2dyb3VuZC1jb2xvcjogeWVsbG93Ow0KfQ0KDQoNCg0K%7C)

Como puedes observar en la imagen, el elemento con la clase yellow tiene un z-index mayor a red, pero no está por encima, porque su contexto de apilamiento está dentro del contexto de apilamiento del elemento blue, así mismo, nunca estará por detrás de su elemento padre

## Propiedades y valores de CSS mas usados

[Documentacion](https://cssreference.io/)

Las propiedades para manipular los textos y tipografía son los siguientes:

1. font-size: establece un tamaño de fuente.
2. font-weight: establece el resaltado del texto, con valores de 100 a 900 en intervalos de 100; donde 100 es delgada y 900 es negrita.
3. font-family: establece el tipo de fuente.
4. text-align: establece la posición del texto: right, left, center y justify.
5. color: establece el color del texto.

## Bordes redondeados

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iYm9yZGVyIj48L2Rpdj4NCjxkaXYgY2xhc3M9ImNpcmNsZSI+PC9kaXY+%7CZGl2IHsNCiAgd2lkdGg6IDIwMHB4Ow0KICBoZWlnaHQ6IDIwMHB4Ow0KICBiYWNrZ3JvdW5kLWNvbG9yOiBicm93bjsNCiAgbWFyZ2luOiAyMHB4Ow0KICBkaXNwbGF5OiBpbmxpbmUtYmxvY2s7DQp9DQoNCi5ib3JkZXJ7DQogIGJvcmRlci1yYWRpdXM6IDM1cHg7DQp9DQoNCi5jaXJjbGV7DQogIGJvcmRlci1yYWRpdXM6IDUwJTsNCn0NCg0KDQo=%7C)

## Unidades de medida

Las unidades de medida establecen una longitud para un determinado elemento o tipografía. Existen dos tipos de medidas: absolutas y relativas.

### Medidas absolutas

Las medidas absolutas son valores fijos, por lo que la medida no cambiará. La unidad absoluta más utilizada son los píxeles px, las demás son muy poco utilizadas, pero es bueno que las conozcas.

### Medidas relativas

Las medidas relativas son valores variables, por lo que la medida depende de un valor externo. Se debe tener en cuidado con estas porque un pequeño cambio puede desencadenar tamaños muy elevados.

- em: el elemento que lo contiene
- rem: el elemento raiz
- vw: 1% del ancho de la pantalla
- vh: 1% de la altura de la pantalla

La medida em depende del elemento que lo contiene, es decir, si un elemento tiene font-size de 20px, el valor de em es igual a 20px, el valor de 2em será de 40px y así sucesivamente.

La medida rem depende del elemento raíz, el valor del font-size del elemento raíz es de 16px, por lo tanto, el valor de 2rem es igual a 32px, y así sucesivamente.

- [Ejemplo em](https://codi.link/PGRpdiBjbGFzcz0ibml2ZWwxIj4NCiAgPHA+TGV0cmEgZGUgMjBweDwvcD4NCiAgPGRpdiBjbGFzcz0ibml2ZWwyIj4NCiAgICA8cD5MZXRyYSBkZSAyMHB4PC9wPg0KICAgIDxkaXYgY2xhc3M9Im5pdmVsMyI+DQogICAgICA8cD5MZXRyYSBkZSA0MHB4PC9wPg0KICAgICAgPGRpdiBjbGFzcz0ibml2ZWw0Ij4NCiAgICAgICAgPHA+TGV0cmEgZGUgODBweDwvcD4NCiAgICAgIDwvZGl2Pg0KICAgIDwvZGl2Pg0KICA8L2Rpdj4NCjwvZGl2Pg==%7CKiB7DQogIG1hcmdpbjogMDsNCn0NCg0KLm5pdmVsMSB7DQogIC8qIFB1ZWRlcyBjYW1iaWFyIGVzdGUgdmFsb3IgKi8NCiAgZm9udC1zaXplOiAyMHB4Ow0KfQ0KDQoubml2ZWwyIHsNCiAgLyogdGFtYcOxbyA9IDIwcHggKiAxID0gMjBweCAqLw0KICBmb250LXNpemU6IDFlbTsNCn0NCg0KLm5pdmVsMyB7DQogIC8qIHRhbWHDsW8gPSAyMHB4ICogMiA9IDQwcHggKi8NCiAgZm9udC1zaXplOiAyZW07DQp9DQoNCi5uaXZlbDQgew0KICAvKiB0YW1hw7FvID0gNDBweCAqIDIgPSA4MHB4ICovDQogIGZvbnQtc2l6ZTogMmVtOw0KfQ0KDQoNCg==%7C)
- [Ejemplo rem](https://codi.link/PGRpdiBjbGFzcz0ibml2ZWwxIj4NCiAgPHA+TGV0cmEgZGUgMjBweDwvcD4NCiAgPGRpdiBjbGFzcz0ibml2ZWwyIj4NCiAgICA8cD5MZXRyYSBkZSAxNnB4PC9wPg0KICAgIDxkaXYgY2xhc3M9Im5pdmVsMyI+DQogICAgICA8cD5MZXRyYSBkZSAzMnB4PC9wPg0KICAgICAgPGRpdiBjbGFzcz0ibml2ZWw0Ij4NCiAgICAgICAgPHA+TGV0cmEgZGUgMzJweDwvcD4NCiAgICAgIDwvZGl2Pg0KICAgIDwvZGl2Pg0KICA8L2Rpdj4NCjwvZGl2Pg==%7CLm5pdmVsMSB7DQogIC8qIFB1ZWRlcyBjYW1iaWFyIGVzdGUgdmFsb3IgKi8NCiAgZm9udC1zaXplOiAyMHB4Ow0KfQ0KDQoubml2ZWwyIHsNCiAgLyogdGFtYcOxbyA9IDE2cHggKiAxID0gMTZweCAqLw0KICBmb250LXNpemU6IDFyZW07DQp9DQoNCi5uaXZlbDMgew0KICAvKiB0YW1hw7FvID0gMTZweCAqIDIgPSAzMnB4ICovDQogIGZvbnQtc2l6ZTogMnJlbTsNCn0NCg0KLm5pdmVsNCB7DQogIC8qIHRhbWHDsW8gPSAxNnB4ICogMiA9IDMycHggKi8NCiAgZm9udC1zaXplOiAycmVtOw0KfQ0KDQoNCg==%7C)

### Diferencias entre porcentajes y la anchura y altura de la pantalla

Los porcentajes representan el tamaño con respecto al total del elemento padre. Si el elemento padre tiene 20px, entonces el 100% será de 20px.

Por otra parte, las medidas de anchura vw y altura vh representan el tamaño con respecto al total de la pantalla. Si el elemento tiene un tamaño de 100vw será el 100 por ciento de la pantalla.

Si un elemento tiene todo el tamaño de la pantalla, entonces solamente en ese punto la medida 100% será igual a 100vw o 100vh.

## Responsive Design

El diseño responsivo (Responsive Design) consiste en un conjunto de herramientas para que tu sitio se vea bien en varias medidas de pantalla, esto incluye imágenes, tipografía, internacionalización de la página y entre otros.

En la actualidad, la mayoría de sitios web son visitados desde un celular, por lo que asegurarse que nuestro sitio sea responsivo para cualquier dispositivo es fundamental para optimizar las ganancias.

### media queries

Las media queries son reglas CSS que establecen un comportamiento distinto o diferentes estilos en un cierto rango de la pantalla. Esto sirve para establecer el layout del sitio web para diferentes tipos de pantalla: escritorio, tablets y celulares.

Estos son dos tipos de media querie :

1. max-width / max-height: establece un rango máximo para cierto comportamiento.
2. min-width / min-height: establece un rango mínimo para cierto comportamiento.

Estos valores son parecidos a condicionales, mientras se cumpla la condición, aplica determinados estilos.

### Estructura

La estructura de una media querie consiste en empezar con @media, seguido del tipo de la media querie estableciendo un rango, envolviendo las reglas CSS dentro de ese rango.

```css
@media (max-width: 750px) {
  div {
    color: red;
  }
  p {
    background-color: red;
  }
}
```

Para observar que los cambios se estén aplicando correctamente, las herramientas de desarrollador serán de gran ayuda.

Abre las herramientas del navegador y da clic en la opción “Toggle device tool”, aquí podrás manipular la pantalla y observar en cuántos píxeles está ocurriendo determinados estilos.

Utiliza el siguiente ejemplo para visualizar cómo cambian los estilos según la longitud de la pantalla. Puedes revisar la media querie que está en el código. Aunque solo cambien el color de dos elementos, puede estar cualquier propiedad que desees, prueba con todo.

[Ejemplo](https://codi.link/PGRpdiBjbGFzcz0iY2FyZDEiPjwvZGl2Pg0KPGRpdiBjbGFzcz0iY2FyZDIiPjwvZGl2Pg0KDQo=%7CKiB7DQogIG1hcmdpbjogMDsNCiAgcGFkZGluZzogMDsNCiAgYm94LXNpemluZzogYm9yZGVyLWJveDsNCn0NCg0KYm9keSB7DQogIHdpZHRoOiAxMDB2dzsNCiAgaGVpZ2h0OiAxMDB2aDsNCn0NCg0KLmNhcmQxew0KICB3aWR0aDogMTAwJTsNCiAgaGVpZ2h0OiAyNSU7DQogIGJhY2tncm91bmQtY29sb3I6IGJyb3duOw0KfQ0KDQouY2FyZDIgew0KICB3aWR0aDogNTAlOw0KICBoZWlnaHQ6IDc1JTsNCiAgYmFja2dyb3VuZC1jb2xvcjogY2hhcnRyZXVzZTsNCn0NCg0KQG1lZGlhIChtaW4td2lkdGg6IDUwMHB4KXsNCiAgLmNhcmQxIHsNCiAgICAgIGJhY2tncm91bmQtY29sb3I6IGNoYXJ0cmV1c2U7DQogIH0NCg0KICAuY2FyZDIgew0KICAgIGJhY2tncm91bmQtY29sb3I6IGJyb3duOw0KICB9DQp9DQoNCg==%7C)

![04](https://miro.medium.com/v2/resize:fit:828/format:webp/1*wbzR91Dii_SN9_GBEKeg1Q.png)

**La mejor forma de aplicar media queries**
Tiene de nombre Mobile First o Mobile Only.
Esto quiere decir que el proyecto ya debe estar diseñado para dispositivos mobile, ya no debemos preocuparnos por que se vea bien desde una laptop o computadora de escritorio. El diseño del proyecto va a partir desde un dispositivo mobile y desde ahí va a ir creciendo a los demás dispositivos con mayor pantalla.

Si hacemos lo contrario de ir de una pantalla grande a una más pequeña, esto se llama solamente responsive design y no es lo que estamos buscando.

**Aplicado directo desde CSS con media queries**

1. Arriba de los media queries vamos a tener el código base, que es el que está hecho y optimizado para dispositivos mobile.
2. Vamos a generar un breakpoint para realizar ciertos cambios en dispositivos más grandes.
3. Vamos a generar otro breakpoint que va a ser para una tablet o para computadoras con un viewport más pequeño como ser netbooks
4. Luego vamos a generar otro breakpoint que será para computadoras de escritorio, desktop o dispositivos con pantallas más grandes.

**Orden para aplicar los media queries**
Partimos desde los dispositivos más pequeños y terminamos con los dispositivos más grandes.
Si lo hacemos de forma inversa tendremos problemas, ya que como CSS funciona en cascada, nunca se van a aplicar los estilos de los medias queries con un viewport más grande.
Empezamos por:

1. Los celulares o dispositivos mobile.
2. Las tablets.
3. Laptops o computadores de escritorio.

**Aplicado directo desde HTML (la mejor practica)**
Este método se utiliza, ya que dependiendo del dispositivo donde esté el usuario va a necesitar un archivo CSS u otro, esto es para evitar que carguen archivos que el usuario no va a necesitar ni usar.

Lo agregamos en el head, aquí en vez de ligar un archivo de CSS vamos a ligar más de uno, dependiendo de los dispositivos en los que queramos aplicar los estilos.

```html
<link rel="stylesheet" href="style.css" />
```

```html
<link rel="stylesheet" href="style.css" />
<link rel="stylesheet" href="tablet.css" media="screen and (min-width:768px)" />
<link
  rel="stylesheet"
  href="desktop.css"
  media="screen and (min-width:1024px)"
/>
```

# Modulo 2: Tailwind CSS

Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite crear rápidamente diseños personalizados y receptivos para sitios web. Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite crear rápidamente diseños personalizados y receptivos para sitios web.

## Mobile first

Mobile first es una técnica de diseño que consiste en diseñar primero la versión móvil de un sitio web, y luego ir agregando características para las versiones de escritorio y tablet.

## Utility first (framework basado en utilidades)

Un framework basado en utilidades es un framework CSS que se basa en clases de utilidad para crear diseños. Por ejemplo, para crear un layout de dos columnas, podemos utilizar las clases de utilidad de Tailwind CSS:

```html
<div class="flex">
  <div class="w-1/2">...</div>
  <div class="w-1/2">...</div>
</div>
```

[Documentacion](https://tailwindcss.com/docs/utility-first)

## Directivas de tailwindcss

[Documentacion](https://tailwindcss.com/docs/functions-and-directives)

## Paleta de colores

[Documentacion](https://tailwindcss.com/docs/customizing-colors)

### Enlaces de interes

1. [Tailwind play](https://play.tailwindcss.com/)
2. [Coolors](https://coolors.co/)

## Medidas y breakpoints

### Width

La propiedad width hace referencia a el ancho del contenedor. La propiedad width puede ser modificada con las siguientes clases:

- w-0 -> width: 0px
- w-px -> width: 1px
- w-4 -> width: 1rem (16px)

**Nota**: de w-1 a w-2 hay un incremento de 0.25rem (4px) de w-1 a w-1.5 hay un incremento de 0.125rem (2px)

- w-auto -> width: auto
- w-1/2 -> width: 50%
- w-1/4 -> width: 25%
- w-full -> width: 100%
- w-screen -> width: 100vw

[Documentacion](https://tailwindcss.com/docs/width)

### Height

la propiedad height hace referencia a el alto del contenedor. La propiedad height puede ser modificada con las siguientes clases:

- h-0 -> height: 0px
- h-px -> height: 1px
- h-4 -> height: 1rem (16px)
- h-1/2 -> height: 50%
- h-1/4 -> height: 25%
- h-full -> height: 100%
- h-screen -> height: 100vh
- h-auto -> height: auto
- h-1/2-screen -> height: 50vh

[Documentacion](https://tailwindcss.com/docs/height)

### Breakpoints

Un breakpoint es un punto en el que se cambia el diseño de una página web. Por ejemplo, en una página web con un diseño de dos columnas, en la versión móvil, las dos columnas se muestran una debajo de la otra, mientras que en la versión de escritorio, las dos columnas se muestran una al lado de la otra.

Podemos utilizar los breakpoints de Tailwind CSS para crear diseños responsivos.

[Breakpoints mas comunes](https://tailwindcss.com/docs/responsive-design)

## Flexbox

[Documentacion](https://tailwindcss.com/docs/flex-direction)

**Nota**: para separar los elementos en el tipo de display flex puedes utilizar space-x-{medida} o gap-{medida}. La diferencia entre space-x y gap es que space-x solo separa los elementos en el eje x, mientras que gap separa los elementos en ambos ejes.

### Algunas propiedades interesantes de flexbox

1. **justify-content**: se utiliza para alinear los elementos horizontalmente
2. **align-items**: se utiliza para alinear los elementos verticalmente

## Plugins oficiales de Tailwind CSS

[Documentacion](https://tailwindcss.com/docs/plugins)

## Aplicacion Platzi Travel

1. Crear carpeta PlatziTravel y crear un proyecto con npm

```bash
npm init -y
```

2. Crear carpeta public y dentro de ella crear el archivo index.html
3. Crear carpeta src y dentro de ella crear el archivo styles.css
4. En la carpeta src crear el archivo index.js
5. Instalar tailwindcss

### Enlaces de interes

1. [Instalacion de Tailwind](https://tailwindcss.com/docs/installation)
2. [Figma](https://www.figma.com/file/aPbr2Rhd5SCUjNYu6NRPPB/Platzi-Travel-Mockups?node-id=0%3A1&mode=dev)
3. [Reppositorio Aplicacion Platzi Travel](https://github.com/platzi/PlatziTravel/tree/main)
4. [Google Fonts](https://fonts.google.com/)

Debes descargar las imagenes y los svg que vamos a utilizar en el proyecto desde el repositorio de github. Los archivos .png y .jpg van en la carpeta public/img y los archivos public/svg van en la carpeta icons.

## Design System

Un Design System es un sistema de diseño que contiene todos los elementos de diseño de una marca, como por ejemplo, los colores, las tipografías, los tamaños, los espaciados, los íconos, etc.

1. Modificar archivo package.json

```js
....
  "scripts": {
	  "tw:build": "npx tailwindcss -i ./src/input.css -o ./dist/output.css",
	  "tw:dev": "npx tailwindcss -i ./src/input.css -o ./dist/output.css --watch",
  },
....
```

2. Modificar tailwind.config.js

```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js}"],
  theme: {
    extend: {
      backgroundImage: {
        sanFrancisco: "url('../img/sanFrancisco.jpg')",
        sanFranciscoDesktop: "url('../img/sanFranciscoDesktop.jpg')",
        yosemite: "url('../img/yosemite.jpg')",
        LA: "url('../img/LA.jpg')",
        seattle: "url('../img/seattle.jpg')",
        new_york: "url('../img/new_york.jpg')",
        norway: "url('../img/norway.jpg')",
        sydney: "url('../img/sydney.jpg')",
        miami: "url('../img/miami.jpg')",
        switzerland: "url('../img/switzerland.jpg')",
        bali: "url('../img/bali.jpg')",
        norway: "url('../img/norway.jpg')",
        chicago: "url('../img/chicago.jpg')",
        europe: "url('../img/europe.jpg')",
        iceland: "url('../img/iceland.jpg')",
      },
      colors: {
        principal: "#CC2D4A",
        secondary: "#8FA206",
        tertiary: "#61AEC9",
      },
      fontFamily: {
        Montserrat: ["Montserrat", "sans-serif"],
      },
    },
  },
  plugins: [],
};
```

Debes buscar en google fonts las fuentes que vamos a utilizar en el proyecto y agregarlas en el archivo index.html. La fuente de este proyecto es Montserrat Regular 400.

```html
<link
  rel="stylesheet"
  href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400&display=swap"
/>
```

## Practica: Seccion Home Mobile

```html
<div class="w-full h-3/4" id="home">
  <div class=" w-full h-full flex flex-col items-center py-4 space-y-96">
    <input
      class="p-3 outline-none rounded-full shadow-lg"
      type="search"
      name="Searchbar"
      placeholder="San Francisco"
      id=""
    />
    <button
      class="bg-white w-48 h-auto p-3 rounded-full shadow-md font-semibold text-principal"
      id="explore-more"
    >
      Explorar
    </button>
  </div>
  <div class="w-full h-full bg-cover">
    <img class="w-full h-full" src="./public/img/sanFrancisco.jpg" alt="" />
  </div>
</div>
```

**Algunas propiedades utilizadas**

1. [flex direction](https://tailwindcss.com/docs/flex-direction)
2. [Alinear elementos verticalmente](https://tailwindcss.com/docs/align-items)
3. [Margen interno: padding](https://tailwindcss.com/docs/padding)
4. [Espacio entre elementos en flex](https://tailwindcss.com/docs/space)
5. [Borde de un elemento](https://tailwindcss.com/docs/outline-style)
6. [Borde redondeado](https://tailwindcss.com/docs/border-radius)
7. [Sombra de caja de un elemento](https://tailwindcss.com/docs/box-shadow)
8. [Color de fondo](https://tailwindcss.com/docs/background-color)
9. [Grosor de la fuente](https://tailwindcss.com/docs/font-weight)
10. [Color de texto](https://tailwindcss.com/docs/text-color)
11. [Tamaño de fondo](https://tailwindcss.com/docs/background-size)

## Practica: Componentes card mobile

```html
<div class="p-20" id="recomendados">
  <div class="w-48 h-64 shadow-md rounded-lg">
    <div
      id="image-container"
      class="w-full h-3/5 rounded-t-lg bg-{nombre_imagen} bg-cover"
    ></div>
    <div class="bg-secondary h-2/5 rounded-b-lg">
      <p class="text-xl px-4 py-2 font-semibold text-white">Noruega</p>
      <p class="text-sm px-4 text-white">Un respiro del mundo</p>
    </div>
  </div>
</div>
```

## Extraccion de componentes a clases

La extracción de componentes sirve para no escribir el mismo código en componentes que se utilizarán más de una vez (ej. cards) y poder mantener el principio de utility-first. La extracción de componentes trabaja de la mano con la directiva **@apply**.

Para hacer la extracción de componentes se procede a lo siguiente:

En el archivo src/css/tailwind.css se crean clases cuyo nombre será el adecuado para identificar cierto componente, dentro de la clase se introducirán todos los estilos de Tailwind que se estarán reutilizando haciendo el uso de la directiva @apply seguido de las clases de Tailwind.

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

.Card {
  @apply w-48 h-64 shadow-md rounded-lg flex-none;
}
```

Haciendo lo anterior se puede utilizar el nombre de la nueva clase en nuestro archivo HTML, es importante ejecutar el script tw:build para que se efectúen los cambios.

```html
<div class="Card">
  <div class="w-full h-3/5 rounded-t-lg bg-norway bg-cover"></div>
  <div class="w-full h-2/5 bg-secondary rounded-b-lg">
    <p class="text-white font-bold text-xl px-4 py-2">Norway</p>
    <p class="text-white px-4">Paisajes Increíbles</p>
  </div>
</div>
```

Cabe mencionar que se deben identificar los componentes que se utilizarán más de una vez en el proyecto ya que Tailwind no está diseñado para trabajar todas nuestras clases de esta manera. Tal como lo menciona la documentación:

Si comienzas a usar @apply para todo, básicamente solo estás escribiendo CSS nuevamente y desechando todas las ventajas del flujo de trabajo y mantenimiento que brinda Tailwind, si va a usar @apply, úsalo para cosas muy pequeñas y altamente reutilizables, como botones y formularios, e incluso, solo si no estás usando un framework como React, donde un componente sería una mejor opción.

[Doumentacion](https://tailwindcss.com/docs/reusing-styles#extracting-classes-with-apply)

## Practica: seccion recomendados mobile

```html
<div class="p-6" id="recomendados">
  <p class="text-3xl font-semibold text-primary">Recomendados</p>
  <div
    class="w-auto h-80 items-center mt-6 overflow-x-auto overscroll-x-contain flex space-x-4"
  >
    <div class="Card">
      <div class="w-full h-3/5 rounded-t-lg bg-norway bg-cover"></div>
      <div class="w-full h-2/5 bg-secondary rounded-b-lg">
        <p class="text-white font-bold text-xl px-4 py-2">Norway</p>
        <p class="text-white px-4">Paisajes Increíbles</p>
      </div>
    </div>
    <div class="Card">
      <div class="w-full h-3/5 rounded-t-lg bg-norway bg-cover"></div>
      <div class="w-full h-2/5 bg-secondary rounded-b-lg">
        <p class="text-white font-bold text-xl px-4 py-2">Norway</p>
        <p class="text-white px-4">Paisajes Increíbles</p>
      </div>
    </div>
    <div class="Card">
      <div class="w-full h-3/5 rounded-t-lg bg-norway bg-cover"></div>
      <div class="w-full h-2/5 bg-secondary rounded-b-lg">
        <p class="text-white font-bold text-xl px-4 py-2">Norway</p>
        <p class="text-white px-4">Paisajes Increíbles</p>
      </div>
    </div>
  </div>
</div>
```

**Algunas propiedades utilizadas**

1. [Scroll](https://tailwindcss.com/docs/overflow)
2. [Scroll 2](https://tailwindcss.com/docs/overscroll-behavior)

## Animaciones con tailwind

```html
<button
  class=".... transition ease-in-out delay-500 hover:-translate-y-1 hover:scale-110 hover:bg-primary hover:text-white"
  id="explore-more"
>
  Explorar
</button>
```

**Algunas propiedades utilizadas**

1. [Primera animacion con tailwind](https://tailwindcss.com/docs/transition-property)
2. [Trasladar un elemento con transformacion](https://tailwindcss.com/docs/translate)
3. [aumentar tamaño del elementos animacion](https://tailwindcss.com/docs/scale)

**transform**: Habilita la transformación CSS en el elemento. Esto es necesario para aplicar las clases relacionadas con transformaciones, como hover:-translate-y-1 y hover:scale-110

**transition-all**: Aplica la transición a todas las propiedades CSS, lo que significa que cualquier cambio en el estilo del botón será animado con la transición definida anteriormente.

## Focus

En Tailwind CSS, la clase focus se utiliza para aplicar estilos específicamente cuando un elemento tiene el enfoque. Este enfoque puede ocurrir, por ejemplo, cuando un usuario interactúa con un elemento utilizando el teclado (por ejemplo, al navegar por la página utilizando la tecla "Tab"). Cuando aplicas la clase focus en Tailwind CSS, estás indicando que los estilos asociados a esa clase deben aplicarse cuando el elemento está enfocado. Por ejemplo, puedes tener una clase como focus:outline-none, que quitará el contorno predeterminado que aparece al enfocar un elemento. Esto puede ser útil para mejorar la accesibilidad y proporcionar una experiencia de usuario más limpia.

### Focus within

En Tailwind CSS, la clase `focus-within` se utiliza para aplicar estilos a un elemento cuando cualquier elemento descendiente de ese elemento tiene el enfoque. Esto es útil cuando deseas estilizar un contenedor basándote en el estado de los elementos hijos que están enfocados.

Por ejemplo, si tienes un contenedor que contiene varios elementos y deseas aplicar estilos al contenedor cuando alguno de sus elementos hijos tiene el enfoque, puedes usar la clase `focus-within`.

**Ejemplo**

```html
<div class="focus-within:bg-gray-200">
  <label for="username">Nombre de usuario:</label>
  <input type="text" id="username" class="focus:outline-none" />
</div>
```

En este ejemplo, el fondo del contenedor cambiará a gris (`bg-gray-200`) cuando el input con `id="username"` está enfocado. La clase `focus-within` se aplica al contenedor y se combina con la clase de color de fondo específica (`bg-gray-200`). También se utiliza la clase `focus:outline-none` en el input para quitar el contorno predeterminado cuando está enfocado.

En resumen, `focus-within` es útil para aplicar estilos al contenedor basándote en el estado de enfoque de sus elementos hijos.

## Ring

En Tailwind CSS, la clase `ring` se utiliza para aplicar un anillo de color alrededor de un elemento. Esto es útil para resaltar un elemento cuando está enfocado, activo o seleccionado.

Por ejemplo, puedes tener una clase como `ring-2` que aplicará un anillo de 2px de ancho alrededor de un elemento.

```html
<input
  class="w-3/4 text-center rounded-full outline-none p-3 shadow-sm transition ease-in-out duration-500 focus-within:shadow-sm focus:ring-2 transform focus:scale-x-105"
  placeholder="San Francisco"
  type="search"
  id=""
/>

....
<div
  class="w-auto h-80 items-center mt-6 overflow-x-auto overscroll-x-contain overflow-y-hidden flex space-x-4"
>
  ....
</div>
```

Agregar una animacion a las card

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

.Card {
  @apply w-48 h-64 shadow-md rounded-lg flex-none transition hover:-translate-y-4 hover:shadow-xl;
}
```

## Practica: seccion rentas destacadas

```html
<div class="px-6 h-full w-full" id="rentas_destacadas">
  <p class="text-3xl text-primary font-semibold pb-6 mt-2">Rentas destacadas</p>
  <div
    class="w-full h-full flex flex-col space-y-4 items-center justify-center"
  >
    <div class="w-full h-96 bg-chicago bg-cover rounded-xl">
      <p class="CardTitle">Chicago</p>
      <p class="text-sm pl-8 text-black mr-24">2 habitaciones, baño y cocina</p>
    </div>
    <div class="w-full h-96 bg-chicago bg-cover rounded-xl">
      <p class="CardTitle">Chicago</p>
      <p class="text-sm pl-8 text-black mr-24">2 habitaciones, baño y cocina</p>
    </div>
  </div>
</div>
```

```css
@tailwind base;
@tailwind components;
@tailwind utilities;

.Card {
  @apply w-48 h-64 shadow-md rounded-lg flex-none transform transition-all hover:-translate-y-4 hover:shadow-xl;
}

.CardTitle {
  @apply text-3xl px-8 pt-8 pb-2 font-semibold text-white;
}
```

## Practica: seccion preguntas frecuentes

```html
<div class="w-full h-full px-6" id="faqs">
  <div class="w-full h-full flex flex-col space-y-4">
    <p class="text-3xl text-primary font-semibold mt-6">FAQs</p>
    <div>
      <p class="text-xl font-semibold text-primary">Política de Cancelación</p>
      <p class="font-medium pt-2">
        Para estancias menores a una semana es importante avisar con 3 días de
        anticipación, de caso contario será sancionado.
      </p>
    </div>
    <div>
      <p class="text-xl font-semibold text-primary">Métodos de pago</p>
      <p class="font-medium pt-2">
        Aceptamos distintos métodos de pago: VISA, MasterCard, American Express,
        Paypal y Binance.
      </p>
    </div>
    <div>
      <p class="text-xl font-semibold text-primary">Mascotas</p>
      <p class="font-medium pt-2">
        El tema de las mascotas dependerá directamente del anfitrión.
      </p>
    </div>
    <div>
      <p class="text-xl font-semibold text-primary">Información de Seguridad</p>
      <p class="font-medium pt-2">
        Todas nuestras estancias cuentan con seguro en caso de accidentes.
      </p>
    </div>
    <div>
      <p class="text-xl font-semibold text-primary">Estancias Largas</p>
      <p class="font-medium pt-2">
        Contamos con estancias de hasta 3 meses, en este caso es requerido un
        anticipo con un monto del 50% del valor de la renta.
      </p>
    </div>
  </div>
</div>
```

## Practica: seccion footer

```html
<footer class="w-full h-auto bg-gray-50 px-6 space-y-2 mt-6 pt-4">
  <p class="text-lg">Acerca De</p>
  <p class="text-sm text-gray-300">Inversionistas</p>
  <p class="text-sm text-gray-300">Empleos</p>
  <p class="text-sm text-gray-300">Términos y condiciones</p>
  <p class="text-sm text-gray-300">Platzi Travel, Inc.</p>
</footer>
```

## Practica: TabBar

```html
<div class="w-full h-16 bg-white fixed left-0 bottom-0 shadow-md flex items-center justify-around" id="tab_bar">
   <a href="#home">
    <svg width="30" height="30" viewBox="0 0 20 20" fill="none" xmlns="">
  ....
</div>
```

## Practica: responsive design

```html
<div id="home">
  <div class="w-full h-3/4">
    <div
      class="w-full h-full flex flex-col absolute space-y-96 py-4 items-center lg:space-y-0 lg:items-start lg:pt-20 lg:justify-start"
    >
      <input
        type="search"
        class="outline-none p-3 rounded-full shadow-sm transition duration-300 focus-within:shadow-sm focus:ring-2 focus:w-11/12 lg:hidden"
        placeholder="San Francisco"
        name=""
        id=""
      />
      <div class="hidden h-auto lg:w-2/5 lg:flex pb-6">
        <p class="text-4xl ml-16 font-bold text-black">
          Encuentra más ubicaciones como esta
        </p>
      </div>
      <button
        class="w-48 rounded-full text-lg text-primary shadow-sm font-semibold p-4 bg-white transition transition-all duration-500 ease-in-out hover:bg-primary hover:text-white transform hover:-translate-y-1 hover:scale-110 lg:ml-16"
      >
        Explorar
      </button>
    </div>
    <div
      class="w-full h-full lg:h-96 lg:bg-sanFranciscoDesktop lg:bg-cover lg:bg-center"
    >
      <img
        class="lg:hidden"
        src="./img/sanFrancisco.jpg"
        alt="San Francisco City"
      />
    </div>
  </div>
</div>
```

```html
<div class="px-6 w-auto lg:px-6" id="rentas_destacadas">
  <p class="text-3xl text-primary font-semibold pb-6 mt-2">Rentas destacadas</p>
  <div class="w-full h-full flex flex-col items-center justify-center">
    <div class="w-full h-96 bg-chicago bg-cover rounded-xl mb-6 lg:bg-center">
      <p class="CardTitle lg:text-b">Chicago</p>
      <p class="text-sm pl-8 text-white mr-24 lg:text-lg">
        2 habitaciones, baño y cocina
      </p>
    </div>
    <div class="lg:flex lg:h-full lg:w-full lg:space-x-4">
      <div class="w-full h-96 bg-LA bg-cover rounded-xl mb-6 lg:h-auto">
        <p class="CardTitle">Los Angeles</p>
        <p class="text-sm pl-8 text-white mr-24 lg:text-lg">
          3 habitaciones, 2 baños, cocina y excelente vista al mar.
        </p>
      </div>
      <div class="h-full w-full">
        <div class="w-full h-96 bg-miami bg-cover rounded-xl mb-6">
          <p class="CardTitle">Miami</p>
          <p class="text-sm pl-8 text-white mr-24 lg:text-lg">
            4 habitaciones, 3 baños, cocina y piscina privada
          </p>
        </div>
        <div class="w-full h-96 bg-bali bg-cover rounded-xl mb-6">
          <p class="CardTitle">Bali</p>
          <p class="text-sm pl-8 text-white mr-24 lg:text-lg">
            2 habitaciones, baño, cocina y piscina privada
          </p>
        </div>
      </div>
    </div>
  </div>
</div>
```

## Practica: creando la navbar

```html
<nav class="w-full h-14 hidden bg-white lg:flex p-4 justify-between">
      <div class="h-auto w-auto">
          <p class="text-xl text-primary font-black">Platzi Travel</p>
      </div>
      <div class="flex space-x-8">
          <a class="font-bold text-base text-primary" href="#home">Inicio</a>
          <a class="font-bold text-base text-primary" href="#recomendados">Recomendados</a>
          <a class="font-bold text-base text-primary" href="#rentas_destacadas">Rentas</a>
          <a class="font-bold text-base text-primary" href="#faqs">FAQs</a>
          <a class="font-bold text-base text-primary" href="#sobre_nosotros">Sobre nosotros</a>
      </div>
      <div class="flex space-x-4">
          <svg width="20" height="20" ... /></svg>
          <svg width="20" height="20" .../></svg>
          <svg width="20" height="20" .../></svg>
      </div>
  </nav>

  <section class="w-full lg:h-screen">
      <div class="lg:w-full lg:h-3/4" id="home">
          <div class="w-full lg:h-full">
              <div class="w-full h-full flex flex-col absolute space-y-96 py-4 items-center lg:space-y-0 lg:items-start lg:pt-48 lg:justify-start">
                  <input type="search" class="outline-none p-3 rounded-full shadow-sm transition duration-300 focus-within:shadow-sm focus:ring-2 focus:w-11/12 lg:hidden" placeholder="San Francisco" name="" id="">
                  <div class="hidden h-auto lg:w-2/5 lg:flex pb-6">
                      <p class="text-4xl ml-16 font-bold text-black">Encuentra más ubicaciones como esta</p>
                  </div>
                  <button class="w-48 rounded-full text-lg text-primary shadow-sm font-semibold p-4 bg-white transition transition-all duration-500 ease-in-out hover:bg-primary hover:text-white transform hover:-translate-y-1 hover:scale-110 lg:ml-16">Explorar</button>
              </div>
              <div class="w-full h-full lg:h-full lg:bg-sanFranciscoDesktop lg:bg-cover lg:bg-center">
                  <img class="lg:hidden" src="./img/sanFrancisco.jpg" alt="San Francisco City">
              </div>
          </div>
      </div>
  </section>
```

## Dark mode

[Documentacion](https://tailwindcss.com/docs/dark-mode)

## Preparando para produccion

[Documentacion](https://tailwindcss.com/docs/optimizing-for-production)

## Migrar desde tailwindcss 2.x a 3.x

[Documentacion](https://tailwindcss.com/docs/upgrade-guide#configure-content-sources)

# Modulo 3: ReactJS

## Enlaces de interes

1. [Repositorio Aplicacion ToDos](https://github.com/platzi/curso-react-intro)
2. [Figma Aplicacion ToDos](https://www.figma.com/file/3aZkIjXMEzBDACmWxqUVes/TODO-Machine-Mockup?node-id=0%3A1&mode=dev)
3. [Figma 2 Aplicacion ToDos](https://www.figma.com/proto/3aZkIjXMEzBDACmWxqUVes/TODO-Machine-Mockup?type=design&amp%3Bnode-id=1-3&amp%3Bt=NH0HT6nS2TxaLKp4-1&amp%3Bscaling=min-zoom&amp%3Bpage-id=0%3A1&amp%3Bstarting-point-node-id=1%3A3&amp%3Bmode=design&node-id=1-3&starting-point-node-id=1%3A3)

## Que es ReactJS

React es una biblioteca de JavaScript de código abierto diseñada para crear interfaces de usuario con el objetivo de facilitar el desarrollo de aplicaciones en una sola página. Es mantenido por Facebook y la comunidad de software libre, han participado en el proyecto más de mil desarrolladores diferentes.

## Que es un componente

Un componente es una pieza de código reutilizable que se puede utilizar para construir elementos de interfaz de usuario. Los componentes son como funciones de JavaScript. Aceptan entradas arbitrarias (llamadas "props") y devuelven elementos React que describen lo que debería aparecer en la pantalla.

[¿Cuándo crear un Componente? Estructura, Organización y Tipos de Componentes en React](https://platzi.com/blog/estructura-organizacion-y-tipos-de-componentes-en-react/)

## Que son Props

En ReactJS, "props" es una abreviatura de "propiedades" (properties en inglés). Las props son un mecanismo fundamental que permite pasar datos desde un componente padre a un componente hijo en una jerarquía de componentes. Es una forma de comunicación unidireccional, lo que significa que los datos fluyen desde el componente padre hacia los componentes hijos, pero no al revés.

Cuando se crea un componente en React, se pueden definir propiedades o props que actúan como variables que el componente recibe y utiliza para renderizar su contenido de manera dinámica. Las props son inmutables, lo que significa que no pueden ser modificadas por el componente hijo, solo pueden ser leídas.

Aquí hay un ejemplo simple para ilustrar el uso de props:

Supongamos que tienes un componente llamado "Saludo" que muestra un mensaje de saludo y recibe el nombre del usuario como prop:

```jsx
import React from "react";

const Saludo = (props) => {
  return <p>Hola, {props.nombre}!</p>;
};

export default Saludo;
```

Luego, en otro componente superior (padre), puedes utilizar el componente "Saludo" y pasarle la prop "nombre":

```jsx
import React from "react";
import Saludo from "./Saludo";

const App = () => {
  return (
    <div>
      <h1>¡Bienvenido a mi aplicación!</h1>
      <Saludo nombre="Juan" />
    </div>
  );
};

export default App;
```

En este ejemplo, el componente "App" es el componente padre que contiene el componente "Saludo" como hijo. El componente "Saludo" recibe la prop "nombre" desde el componente padre y lo utiliza para mostrar el mensaje "Hola, Juan!" en el navegador.

Las props son una forma eficiente de pasar datos y configuraciones entre componentes en una aplicación React, lo que permite crear componentes reutilizables y modulares que pueden adaptarse a diferentes contextos mediante el uso de diferentes props.

## Estilos con React

Puedes usar estilos de CSS en React de dos formas:

- **Estilos en línea**: se aplican directamente a un elemento usando el atributo style.

```jsx
const estilos = {
  fontSize: "24px",
  textAlign: "center",
  margin: "0",
  padding: "48px",
};

function ToDoCounter({ total, completed }) {
  return (
    <h1 style={estilos}>
      Has completado {completed} de {total} TODOS
    </h1>
  );
}

export { ToDoCounter };
```

- **Utilizando archivos .css**: se crean archivos .css que contienen los estilos y luego se importan en los componentes que los necesitan.

```css
/* ./ToDoCounter.css */
h1 {
  font-size: 24px;
  text-align: center;
  margin: 0;
  padding: 48px;
}
```

```jsx
import "./ToDoCounter.css";

function ToDoCounter({ total, completed }) {
  return (
    <h1>
      Has completado {completed} de {total} TODOS
    </h1>
  );
}

export { ToDoCounter };
```

En CSS, podemos incluir o quitar estilos de un elemento de forma dinamica utilizando clases.

```jsx
...
function ToDoItem(props) {
  return (
      <li className="TodoItem">
        <span className={`Icon Icon-check ${props.completed && "Icon-check--active"}`}>
        V
        </span>
      ...
      </li>
  );
}
```

En este ejemplo, la clase "Icon-check--active" solo se aplicará cuando la prop "completed" sea verdadera.

```css
.Icon-check {
  position: absolute;
  left: 12px;
}
.Icon-check--active {
  color: #4caf50;
}
```

```jsx
import "./TodoItem.css";

function TodoItem(props) {
  return (
    <li className="TodoItem">
      <span
        className={`Icon Icon-check ${props.completed && "Icon-check--active"}`}
      >
        V
      </span>
      <p className={`TodoItem-p ${props.completed && "TodoItem-p--complete"}`}>
        {props.text}
      </p>
      <span className="Icon Icon-delete">X</span>
    </li>
  );
}

export { TodoItem };
```

```css
.TodoItem {
  background-color: #fafafa;
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 24px;
  box-shadow: 0px 5px 50px rgba(32, 35, 41, 0.15);
}

.TodoItem-p {
  margin: 24px 0 24px 24px;
  width: calc(100% - 120px);
  font-size: 18px;
  line-height: 24px;
  font-weight: 400;
}
.TodoItem-p--complete {
  text-decoration: line-through;
}

.Icon {
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 48px;
  width: 48px;
  font-size: 24px;
  font-weight: bold;
  /* background-color: #CCC; */
}

.Icon-check {
  position: absolute;
  left: 12px;
}
.Icon-check--active {
  color: #4caf50;
}

.Icon-delete {
  position: absolute;
  top: -24px;
  right: 0;
}
.Icon-delete:hover {
  color: red;
}
```

### Enlaces de interes

1. [Estilos componentes Aplicacion ToDo](https://github.com/platzi/curso-react-intro/tree/04-css)
2. [Google Fonts](https://fonts.google.com/)

## Eventos con ReactJS

Los eventos son acciones que suceden en el navegador que pueden ser detectadas por React y utilizadas para ejecutar código cuando ocurren. Algunos ejemplos de eventos son: hacer clic en un botón, pasar el mouse sobre un elemento, escribir en un campo de texto, etc.

### onClick

Se ejecuta cuando se hace clic en un elemento.

```jsx
import "./CreateToDoButton.css";

function CreateToDoButton() {
  return (
    <button
      className="CreateToDoButton"
      onClick={() => {
        console.log("Le diste click");
      }}
    >
      +
    </button>
  );
}

export { CreateToDoButton };
```

### onChange

Se ejecuta cuando el valor de un elemento cambia, como un campo de texto.

```jsx
import "./ToDoSearch.css";

function ToDoSearch() {
  return (
    <input
      placeholder="Cortar cebolla"
      className="TodoSearch"
      onChange={(event) => {
        console.log(event.target.value);
      }}
    />
  );
}

export { ToDoSearch };
```

**Nota**: event.target hace referencia al elemento que disparo el evento. event.target.value se usa para obtener el valor actual del elemento de entrada.

## Estados

Los componentes de React tienen un objeto llamado state, que es donde se almacena y actualiza la información que se utiliza para renderizar el componente. El estado es un objeto que contiene los datos relevantes para un componente y puede cambiar a lo largo del tiempo. Cuando el estado de un componente cambia, React vuelve a renderizar el componente.

Para crear un estado en un componente, se utiliza el método useState, que devuelve un arreglo con dos elementos: el estado actual y una función que se utiliza para actualizar el estado.

```jsx
import React from "react";
import "./ToDoSearch.css";

function ToDoSearch() {
  const [searchValue, setSearchValue] = React.useState(''); // Estado inicial

  console.log('Los usuarios buscan todos de ' + searchValue');

  return (
    <input
      placeholder="Cortar cebolla"
      className="TodoSearch"
      value={searchValue} // Valor del estado
      onChange={(event) => {
        console.log(event.target.value);
        setSearchValue(event.target.value);
      }}
    />
  );
}

export { ToDoSearch };
```

### Practica: Estados

1. el primer reto consiste en actualizar el valor de los ToDos completados en el componente padre App.Para empezar hay que aclarar que los estados se definen en el componente padre, en este caso App, y se pasan como props a los componentes hijos. Para actualizar el estado desde un componente hijo, se debe pasar la función que actualiza el estado como prop al componente hijo, y luego llamar a esa función desde el componente hijo. Veamos.

```jsx
...

const defaultToDos = [
  { text: "Cortar cebolla", completed: true },
  { text: "Tomar el curso de intro a React", completed: false },
  { text: "Llorar con la llorona", completed: false },
  { text: "LALALA", completed: false },
]

function App() {
  const [toDos, setToDos] = React.useState(defaultToDos);
  const [searchValue, setSearchValue] = React.useState('');

  console.log('Los usuarios buscan todos de ' + searchValue);

  return (
    <>
      <ToDoCounter completed={completedToDos} total={totalToDos} />
      <ToDoSearch
        searchValue={searchValue} // Valor del estado
        setSearchValue={setSearchValue} // Funcion que actualiza el estado
      />
      ...
  );
}
```

```jsx
..
function ToDoSearch({
  searchValue, // Valor del estado
  setSearchValue, // Funcion que actualiza el estado
}) {
  return (
    <input
      placeholder="Cortar cebolla"
      className="TodoSearch"
      value={searchValue} // Valor del estado
      onChange={(event) => {
        console.log(event.target.value);
        setSearchValue(event.target.value);
      }}
    />
  );
}
...
```

2. El segundo reto consiste en realizar el conteo de ToDos de forma dinamica

```jsx
import { ToDoCounter } from "./ToDoCounter";
import { ToDoSearch } from "./ToDoSearch";
import { ToDoList } from "./ToDoList";
import { ToDoItem } from "./ToDoItem";
import { CreateToDoButton } from "./CreateToDoButton";
import "./App.css";
import React from "react";

const defaultToDos = [
  { text: "Cortar cebolla", completed: true },
  { text: "Tomar el curso de intro a React", completed: false },
  { text: "Llorar con la llorona", completed: false },
  { text: "LALALA", completed: false },
];

function App() {
  const [toDos, setToDos] = React.useState(defaultToDos);
  const [searchValue, setSearchValue] = React.useState("");

  const completedToDos = toDos.filter((toDo) => toDo.completed).length;
  const totalToDos = toDos.length;

  console.log("Los usuarios buscan todos de " + searchValue);

  return (
    <>
      <ToDoCounter completed={completedToDos} total={totalToDos} />
      <ToDoSearch searchValue={searchValue} setSearchValue={setSearchValue} />
      <ToDoList>
        {defaultToDos.map((toDo, index) => (
          <ToDoItem key={index} text={toDo.text} completed={toDo.completed} />
        ))}
      </ToDoList>
      <CreateToDoButton />
    </>
  );
}

export default App;
```

3. El tercer reto consiste en filtrar los ToDos de acuerdo a la busqueda del usuario

```jsx
...

function App() {
  const [toDos, setToDos] = React.useState(defaultToDos);
  const [searchValue, setSearchValue] = React.useState('');

  const searchedToDos = toDos.filter((toDo) => {
    const toDoText = toDo.text.toLowerCase();
    const searchValueText = searchValue.toLowerCase();
    return toDoText.includes(searchValueText);
  });

  return (
    <>
      ...
      <ToDoSearch
        searchValue={searchValue}
        setSearchValue={setSearchValue}
      />
      <ToDoList>
        {searchedToDos.map((toDo, index) => (
          <ToDoItem key={index} text={toDo.text} completed={toDo.completed} />
        ))}
      </ToDoList>
      <CreateToDoButton />
    </>
  );
}

export default App;
```

1. El cuarto reto consiste en completar los ToDos

```jsx
...

function App() {
  ...

  const completeToDo = (text) => {
    const newToDos = [...toDos];
    const toDoIndex = newToDos.findIndex((toDo) => toDo.text === text);
    newToDos[toDoIndex].completed = true;
    setToDos(newToDos);
  }

  return (
    <>
      <ToDoCounter completed={completedToDos} total={totalToDos} />
      <ToDoSearch searchValue={searchValue} setSearchValue={setSearchValue} />
      <ToDoList>
        {searchedToDos.map((toDo, index) => (
          <ToDoItem
            key={index}
            text={toDo.text}
            completed={toDo.completed}
            onComplete={() => completeToDo(toDo.text)}
          />
        ))}
      </ToDoList>
      <CreateToDoButton />
    </>
  );
}

export default App;
```

```jsx
import "./ToDoItem.css";

function ToDoItem(props) {
  return (
    <li className="TodoItem">
      <span
        className={`Icon Icon-check ${props.completed && "Icon-check--active"}`}
        onClick={() => props.onComplete(props.text)}
      >
        V
      </span>
      ...
    </li>
  );
}
export { ToDoItem };
```

5. El quinto reto consiste en eliminar los ToDos

```jsx
...
function App() {
  ...

  const deleteToDo = (text) => {
    const newToDos = [...toDos];
    const toDoIndex = newToDos.findIndex((toDo) => toDo.text === text);
    newToDos.splice(toDoIndex, 1);
    setToDos(newToDos);
  }

  return (
    <>
      <ToDoCounter completed={completedToDos} total={totalToDos} />
      <ToDoSearch searchValue={searchValue} setSearchValue={setSearchValue} />
      <ToDoList>
        {searchedToDos.map((toDo, index) => (
          <ToDoItem
            key={index}
            text={toDo.text}
            completed={toDo.completed}
            onComplete={() => completeToDo(toDo.text)}
            onDelete={() => deleteToDo(toDo.text)}
          />
        ))}
      </ToDoList>
      <CreateToDoButton />
    </>
  );
}

export default App;
```

```jsx
import './ToDoItem.css'

function ToDoItem(props) {
  return (
      ...
      <span className="Icon Icon-delete"
      onClick={props.onDelete}>X</span>
    </li>
  );
}
export { ToDoItem };
```

## Iconos

### Librerias de terceros

Existen diferentes librerias de iconos que podemos utilizar en nuestros proyectos de React,una de las mas populares es React Icons, que nos permite utilizar iconos de diferentes librerias como Font Awesome, Material Design, Ionicons, etc.:

[React Icons](https://react-icons.github.io/react-icons/)

Aveces, no se puede utilizar iconos de librerias por que desde el area de diseño nos entregan iconos personalizados. En estos casos, podemos 'crear nuestra propia libreria de iconos' utilizando componentes de React. **Primero debes incluir los svg en la carpeta src.**

**Nota**: si quieres iconos dinamicos, por ejemplo, que cambien de color, debes quitar en cada archivo svg
debes eliminar la propiedad fill y posteriormente, incluirla con ReactJS como lo vamos hacer.

### Libreria de iconos personalizados

1. Crear TodoIcon.js. Este componente recibe como prop el tipo de icono que se va a renderizar y el color del icono.

```jsx
// src/TodoIcon.js
import { ReactComponent as CheckSVG } from "./check.svg";
import { ReactComponent as DeleteSVG } from "./delete.svg";
import "./TodoIcon.css";

const iconTypes = {
  check: <CheckSVG />,
  delete: <DeleteSVG />,
};

function TodoIcon({ type }) {
  return (
    <span className={`Icon-container Icon-container-${type}`}>
      {iconTypes[type]}
    </span>
  );
}

export { TodoIcon };
```

```jsx
import React from "react";
import { TodoIcon } from "./TodoIcon";

function CompleteIcon() {
  return <TodoIcon type="check" />;
}

export { CompleteIcon };
```

```jsx
import React from "react";
import { TodoIcon } from "./TodoIcon";

function DeleteIcon() {
  return <TodoIcon type="delete" />;
}

export { DeleteIcon };
```

2. Crear la propiedad color en ToDoIcon.js y incluir la clase Icon-svg a cada svg, ademas de modificarlos para recibir el parametro color y finalmnente incluir la propiedad fill.

```jsx
// src/TodoIcon.js
import { ReactComponent as CheckSVG } from "./check.svg";
import { ReactComponent as DeleteSVG } from "./delete.svg";
import "./TodoIcon.css";

const iconTypes = {
  check: (color) => <CheckSVG className="Icon-svg" fill={color} />,
  delete: (color) => <DeleteSVG className="Icon-svg" fill={color} />,
};

function TodoIcon({ type, color, onClick }) {
  return (
    <span className={`Icon-container Icon-container-${type}`} onClick={onClick}>
      {iconTypes[type](color)}
    </span>
  );
}

export { TodoIcon };
```

```jsx
import React from "react";
import { TodoIcon } from "./TodoIcon";

function CompleteIcon({ completed, onComplete }) {
  return (
    <TodoIcon
      type="check"
      color={completed ? "green" : "gray"}
      onClick={onComplete}
    />
  );
}

export { CompleteIcon };
```

```jsx
import React from "react";
import { TodoIcon } from "./TodoIcon";

function DeleteIcon({ onDelete }) {
  return <TodoIcon type="delete" color="gray" onClick={onDelete} />;
}

export { DeleteIcon };
```

Estos son los estilos del componente TodoIcon

```css
.Icon-container {
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 48px;
  width: 48px;
  font-size: 24px;
  font-weight: bold;
  /* background-color: #CCC; */
}

.Icon-container-check {
  position: absolute;
  left: 12px;
}
.Icon-container-check--active {
  color: #4caf50;
}

.Icon-container-delete {
  position: absolute;
  top: -24px;
  right: 0;
}

.Icon-svg {
  width: 24px;
  height: 24px;
}

.Icon-container-check:hover .Icon-svg {
  fill: green;
}
.Icon-container-delete:hover .Icon-svg {
  fill: red;
}
```

Este es el codigo del ToDoItem

```jsx
import { CompleteIcon } from "./CompleteIcon";
import { DeleteIcon } from "./DeleteIcon";
import "./TodoItem.css";

function TodoItem(props) {
  return (
    <li className="TodoItem">
      <CompleteIcon completed={props.completed} onComplete={props.onComplete} />

      <p className={`TodoItem-p ${props.completed && "TodoItem-p--complete"}`}>
        {props.text}
      </p>

      <DeleteIcon onDelete={props.onDelete} />
    </li>
  );
}

export { TodoItem };
```

## LocalStorage

Es una API que nos permite almacenar datos en el navegador de forma persistente. Los datos almacenados en el localStorage no se eliminan al cerrar el navegador, ni al apagar el computador, ni al reiniciar el sistema operativo. Los datos almacenados en el localStorage permanecen ahí hasta que se borren manualmente, o hasta que se borren utilizando código.

Para acceder al localStorage, lo podemos hacer desde la consola del navegador, utilizando el objeto localStorage. Por ejemplo, para guardar un dato en el localStorage, podemos utilizar el método setItem:

```jsx
localStorage.setItem("nombre", "Juan");
```

Para obtener un dato del localStorage, podemos utilizar el método getItem:

```jsx
localStorage.getItem("nombre");
```

Para eliminar un dato del localStorage, podemos utilizar el método removeItem:

```jsx
localStorage.removeItem("nombre");
```

En nuestro proyecto, vamos a utilizar el localStorage para guardar los ToDos, de forma que cuando el usuario recargue la página, los ToDos se sigan mostrando.

1. En la consola del navegador vas a crear el array de objetos que contiene los ToDos, y lo vas a guardar en el localStorage utilizando el método setItem:

```jsx
const defaultTodos = [
  { text: "Cortar cebolla", completed: true },
  { text: "Tomar el curso de intro a React", completed: false },
  { text: "Llorar con la llorona", completed: false },
  { text: "LALALA", completed: false },
];

localStorage.setItem("TODOS_V1", JSON.stringify(defaultTodos));
```

**Nota**: Todo lo que se guarda en localStorage debe ser un string.

2. En el componente App, vamos a crear un estado para guardar los ToDos, y lo vamos a inicializar con los ToDos que están guardados en el localStorage:

```jsx
...

// const defaultTodos = [
//   { text: 'Cortar cebolla', completed: true },
//   { text: 'Tomar el Curso de Intro a React.js', completed: false },
//   { text: 'Llorar con la Llorona', completed: false },
//   { text: 'LALALALALA', completed: false },
//   { text: 'Usar estados derivados', completed: true },
// ];

// localStorage.setItem('TODOS_V1', JSON.stringify(defaultTodos));
// localStorage.removeItem('TODOS_V1');

function App() {
  const localStorageTodos = localStorage.getItem('TODOS_V1');

  let parsedTodos;

  // Si no hay ToDos en localStorage, entonces parsedTodos será un array vacío
  if (!localStorageTodos) {
    localStorage.setItem('TODOS_V1', JSON.stringify([]));
    parsedTodos = [];
  } else {
    parsedTodos = JSON.parse(localStorageTodos);
  }

  ...

  const saveTodos = (newTodos) => {
    localStorage.setItem('TODOS_V1', JSON.stringify(newTodos));

    setTodos(newTodos);
  };

  const completeTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text == text
    );
    newTodos[todoIndex].completed = true;
    saveTodos(newTodos);
  };

  const deleteTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text == text
    );
    newTodos.splice(todoIndex, 1);
    saveTodos(newTodos);
  };

  return (
    <>
      <TodoCounter
        completed={completedTodos}
        total={totalTodos}
      />
      <TodoSearch
        searchValue={searchValue}
        setSearchValue={setSearchValue}
      />

      <TodoList>
        {searchedTodos.map(todo => (
          <TodoItem
            key={todo.text}
            text={todo.text}
            completed={todo.completed}
            onComplete={() => completeTodo(todo.text)}
            onDelete={() => deleteTodo(todo.text)}
          />
        ))}
      </TodoList>

      <CreateTodoButton />
    </>
  );
}

export default App;
```

## Custom Hooks

Los Custom Hooks son una característica de React que nos permite extraer lógica de componentes en funciones reutilizables. Por convencion las funciones de custom Hooks comienzan con la palabra _use_

1. Crear el custom hook _useLocalStorage_

```jsx
function useLocalStorage(itemName, initialValue) {
  const localStorageItem = localStorage.getItem(itemName);

  let parsedItem;

  if(!localStorageItem) {
    localStorage.setItem(itemName, JSON.stringify(initialValue));
    parsedItem = initialValue;
  } else {
    parsedItem = JSON.parse(localStorageItem);
  }

  const [item, setItem] = React.useState(parsedItem);

  const saveItem = (newItem) => {
    localStorage.setItem(itemName, JSON.stringify(newItem));
    setItem(newItem);
  };

  return [item, saveItem];
}

function App() {
  const [todos, saveTodos] = useLocalStorage('TODOS_V1', []);
  const [searchValue, setSearchValue] = React.useState('');
  ...

  const completeTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text == text
    );
    newTodos[todoIndex].completed = true;
    saveTodos(newTodos);
  };

  const deleteTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text == text
    );
    newTodos.splice(todoIndex, 1);
    saveTodos(newTodos);
  };

  ...
}

export default App;
```

## Organizacion de archivos

Una buena práctica para organizar los archivos de un proyecto de React es agrupar los archivos relacionados en carpetas. Por ejemplo, en nuestro proyecto, podemos crear una carpeta llamada components, y dentro de esta carpeta crear una carpeta para cada componente. De esta forma, todos los archivos relacionados con un componente estarán en la misma carpeta. Por ejemplo, el componente TodoItem podría tener la siguiente estructura de archivos:

```bash
TodoItem
├── TodoItem.css
├── TodoItem.jsx
├── TodoItem.test.jsx
└── index.js
```

El componente TodoIcon podría tener la siguiente estructura de archivos:

```bash
TodoIcon
├── TodoIcon.css
├── TodoIcon.jsx
├── TodoIcon.test.jsx
├── CompleteIcon.js
├── DeleteIcon.js
├── delete.svg
├── check.svg
└── index.js
```

Para el archivo app, la estructura de archivos podría ser la siguiente:

```bash
App
├── index.js
└── useLocalStorage.js
```

**Nota**: Para poder separar la funcion useLocalStorage debes incluir al final del arhivo la exportacion `export { useLocalStorage };`, para poder importar la funcion useLocalStorage debes incluir al final del arhivo la importacion. `import { useLocalStorage } from './useLocalStorage';`

Tambien puedes mover la UI de tu componente a un archivo separado, por ejemplo.

1. Crear un archivo AppUI.js

```js
// Todos los imports de React y componentes

function AppUI({
  totalTodos,
  completedTodos,
  searchValue,
  setSearchValue,
  searchedTodos,
  completeTodo,
  deleteTodo,
}) {
  return (
    <>
      <TodoCounter completed={completedTodos} total={totalTodos} />
      <TodoSearch searchValue={searchValue} setSearchValue={setSearchValue} />

      <TodoList>
        {searchedTodos.map((todo) => (
          <TodoItem
            key={todo.text}
            text={todo.text}
            completed={todo.completed}
            onComplete={() => completeTodo(todo.text)}
            onDelete={() => deleteTodo(todo.text)}
          />
        ))}
      </TodoList>

      <CreateTodoButton />
    </>
  );
}

export { AppUI };
```

2. Importar el componente AppUI en App.js

```jsx
import { AppUI } from './AppUI';

function App() {
  const [todos, saveTodos] = useLocalStorage('TODOS_V1', []);
  const [searchValue, setSearchValue] = React.useState('');
  ...

  const completeTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text == text
    );
    newTodos[todoIndex].completed = true;
    saveTodos(newTodos);
  };

  const deleteTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text == text
    );
    newTodos.splice(todoIndex, 1);
    saveTodos(newTodos);
  };

  ...

  return (
    <AppUI
      totalTodos={totalTodos}
      completedTodos={completedTodos}
      searchValue={searchValue}
      setSearchValue={setSearchValue}
      searchedTodos={searchedTodos}
      completeTodo={completeTodo}
      deleteTodo={deleteTodo}
    />
  );
}

export default App;
```

## Efectos en React

Los efectos son una característica de React que nos permite ejecutar código cuando se monta, desmonta o actualiza un componente. Los efectos se utilizan para ejecutar código que necesita acceder al DOM, como por ejemplo, para obtener el tamaño de la ventana, o para ejecutar código asíncrono, como por ejemplo, para obtener datos de una API.

### useEffect

Se ejecuta cuando se monta, desmonta o actualiza un componente. Recibe dos parámetros: una función que se ejecuta cuando se monta, desmonta o actualiza el componente, y una lista de dependencias que se utiliza para indicarle a React cuando debe volver a ejecutar la función. Si la lista de dependencias está vacía, la función se ejecuta solo cuando se monta y desmonta el componente.

```jsx
import React from "react";

function App() {
  console.log("Log1");

  React.useEffect(() => {
    console.log("Log2");
  }); // Si no se pasa un arreglo de dependencias, se ejecuta cuando se monta y desmonta el componente

  React.useEffect(() => {
    console.log("Log2");
  }, []); // Si se pasa un arreglo de dependencias vacío, se ejecuta solo cuando se monta el componente

  React.useEffect(() => {
    console.log("Log2");
  }, [totalTodos]); // Si se pasa un arreglo de dependencias con una variable, se ejecuta cuando se monta el componente y cuando cambia el valor de la variable

  console.log("Log3");

  return <div></div>;
}

export default App;
```

Para ejecutar código cuando se desmonta un componente, se debe retornar una función en la función que se pasa como primer parámetro a useEffect:

```jsx
React.useEffect(() => {
  console.log("Log2");

  return () => {
    console.log("Log4");
  };
});
```

useEffect se utiliza comunmente para obtener datos de una API, por ejemplo:

```jsx
import React from "react";

function TodoMessage() {
  const [state, setState] = React.useState({});

  React.useEffect(() => {
    fetch("url")
      .then((response) => response.json())
      .then((data) => setState(data));
  }, []);

  return <p>{state.message} || "Cargando..."</p>;
}

export default TodoMessage;
```

### Practica: Implementando estados de carga y error en la aplicacion ToDos

en el archivo useLocalStorage.js

```jsx
import React from 'react';

function useLocalStorage(itemName, initialValue) {
  const [item, setItem] = React.useState(initialValue);
  const [loading, setLoading] = React.useState(true);
  const [error, setError] = React.useState(false);

  React.useEffect(() => {
    setTimeout(() => {
      try {
        const localStorageItem = localStorage.getItem(itemName);

        let parsedItem;

        if (!localStorageItem) {
          localStorage.setItem(itemName, JSON.stringify(initialValue));
          parsedItem = initialValue;
        } else {
          parsedItem = JSON.parse(localStorageItem);
          setItem(parsedItem);
        }

        setLoading(false);
      } catch(error) {
        setLoading(false);
        setError(true);
      }
    }, 2000);
  , []);

  const saveItem = (newItem) => {
    localStorage.setItem(itemName, JSON.stringify(newItem));
    setItem(newItem);
  };

  return {
    item,
    saveItem,
    loading,
    error,
  };
}

export { useLocalStorage };
```

en el archivo App/index.js

```jsx
...


function App() {
  const {
    item: todos,
    saveItem: saveTodos,
    loading,
    error,
  } = useLocalStorage('TODOS_V1', []);
  const [searchValue, setSearchValue] = React.useState('');

  ...

  return (
    <AppUI
      loading={loading}
      error={error}
      completedTodos={completedTodos}
      totalTodos={totalTodos}
      searchValue={searchValue}
      setSearchValue={setSearchValue}
      searchedTodos={searchedTodos}
      completeTodo={completeTodo}
      deleteTodo={deleteTodo}
    />
  );
}

export default App;
```

Crear componente EmpyTodos

```jsx
import React from "react";

function EmptyTodos() {
  return <p>¡Crea tu primer TODO!</p>;
}

export { EmptyTodos };
```

Crear componente TodosError

```jsx
import React from "react";

function TodosError() {
  return <p>Error...</p>;
}

export { TodosError };
```

Crear componente TodosLoading

```jsx
import React from "react";
import "./TodosLoading.css";

function TodosLoading() {
  return (
    <div className="LoadingTodo-container">
      <span className="LoadingTodo-completeIcon"></span>
      <p className="LoadingTodo-text"></p>
      <span className="LoadingTodo-deleteIcon"></span>
    </div>
  );
}

export { TodosLoading };
```

en el archivo TodosLoading.css

```css
.LoadingTodo-container {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 24px;
  box-shadow: 0px 5px 50px rgba(32, 35, 41, 0.15);
  border-radius: 10px;
  padding: 12px 0;
}

.LoadingTodo-text {
  margin: 24px 0 24px 24px;
  width: calc(100% - 120px);
  font-size: 18px;
  line-height: 24px;
  font-weight: 400;
}

.LoadingTodo-completeIcon,
.LoadingTodo-deleteIcon {
  cursor: pointer;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 50px;
  height: 48px;
  width: 48px;
}
.LoadingTodo-completeIcon {
  position: absolute;
  left: 12px;
}
.LoadingTodo-deleteIcon {
  position: absolute;
  top: -24px;
  right: 0;
}

.LoadingTodo-container,
.LoadingTodo-completeIcon,
.LoadingTodo-deleteIcon {
  background: linear-gradient(
    90deg,
    rgba(250, 250, 250, 1),
    rgb(200, 199, 199)
  );
  background-size: 400% 400%;
  animation: loadingAnimation 3s ease-in-out infinite;
}

@keyframes loadingAnimation {
  0% {
    background-position: 0% 50%;
  }
  50% {
    background-position: 100% 50%;
  }
  100% {
    background-position: 0% 50%;
  }
}
```

en el archivo App/AppUI.js

```jsx
...
import { TodosLoading } from '../TodosLoading';
import { TodosError } from '../TodosError';
import { EmptyTodos } from '../EmptyTodos';
import { CreateTodoButton } from '../CreateTodoButton';

function AppUI({
  loading,
  error,
  completedTodos,
  totalTodos,
  searchValue,
  setSearchValue,
  searchedTodos,
  completeTodo,
  deleteTodo,
}) {
  return (
    <>
      ...
      <TodoList>
        {loading && (
          <>
            <TodosLoading />
            <TodosLoading />
            <TodosLoading />
          </>
        )}
        {error && <TodosError/>}
        {(!loading && searchedTodos.length === 0) && <EmptyTodos />}

        ...
      </TodoList>

      <CreateTodoButton />
    </>
  );
}

export { AppUI };
```

## React Context

Context es una característica de React que nos permite compartir datos entre componentes sin tener que pasar props manualmente entre cada componente. Context es una forma de crear un estado global que puede ser consumido en cualquier componente de la aplicación.

1. Crear el archivo src/TodoContext/index.js

```jsx
import React from "react";
import { useLocalStorage } from "./useLocalStorage";

const TodoContext = React.createContext();

function TodoProvider({ children }) {
  const {
    item: todos,
    saveItem: saveTodos,
    loading,
    error,
  } = useLocalStorage("TODOS_V1", []);
  const [searchValue, setSearchValue] = React.useState("");

  const completedTodos = todos.filter((todo) => !!todo.completed).length;
  const totalTodos = todos.length;

  const searchedTodos = todos.filter((todo) => {
    const todoText = todo.text.toLowerCase();
    const searchText = searchValue.toLowerCase();
    return todoText.includes(searchText);
  });

  const completeTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex((todo) => todo.text === text);
    newTodos[todoIndex].completed = true;
    saveTodos(newTodos);
  };

  const deleteTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex((todo) => todo.text === text);
    newTodos.splice(todoIndex, 1);
    saveTodos(newTodos);
  };

  return (
    <TodoContext.Provider
      value={{
        loading,
        error,
        completedTodos,
        totalTodos,
        searchValue,
        setSearchValue,
        searchedTodos,
        completeTodo,
        deleteTodo,
      }}
    >
      {children}
    </TodoContext.Provider>
  );
}

export { TodoContext, TodoProvider };
```

2. Arrastrar localStorage a TodoContext
3. En el componente AppUI.js importar el contexto

```jsx
...
import { TodoContext } from '../TodoContext';

function AppUI() {
  return (
    <>
      <TodoCounter />
      <TodoSearch />

      <TodoContext.Consumer> // Recibe una funcion
        {({
          loading,
          error,
          searchedTodos,
          completeTodo,
          deleteTodo,
        }) => (
          <TodoList>
            {loading && (
              <>
                <TodosLoading />
                <TodosLoading />
                <TodosLoading />
              </>
            )}
            {error && <TodosError/>}
            {(!loading && searchedTodos.length === 0) && <EmptyTodos />}

            {searchedTodos.map(todo => (
              <TodoItem
                key={todo.text}
                text={todo.text}
                completed={todo.completed}
                onComplete={() => completeTodo(todo.text)}
                onDelete={() => deleteTodo(todo.text)}
              />
            ))}
          </TodoList>
        )}
      </TodoContext.Consumer>

      <CreateTodoButton />
    </>
  );
}

export { AppUI };
```

Otra forma de consumir el contexto es utilizando el hook useContext

En el componente TodoCounter

```jsx
import React from "react";
import { TodoContext } from "../TodoContext";
import "./TodoCounter.css";

function TodoCounter() {
  const { completedTodos, totalTodos } = React.useContext(TodoContext);

  return (
    <h1 className="TodoCounter">
      Has completado <span>{completedTodos}</span> de <span>{totalTodos}</span>{" "}
      TODOs
    </h1>
  );
}

export { TodoCounter };
```

En el componente TodoSearch

```jsx
import React from "react";
import { TodoContext } from "../TodoContext";
import "./TodoSearch.css";

function TodoSearch() {
  const { searchValue, setSearchValue } = React.useContext(TodoContext);

  return (
    <input
      placeholder="Cortar cebolla"
      className="TodoSearch"
      value={searchValue}
      onChange={(event) => {
        setSearchValue(event.target.value);
      }}
    />
  );
}

export { TodoSearch };
```

## React Portals

Los Portales son una característica de React que nos permite renderizar un componente en cualquier parte del DOM, incluso fuera del contenedor principal de la aplicación. Se utilizan para renderizar componentes que deben estar por encima de otros componentes, como por ejemplo, los modales.

1. Crear el archivo src/Modal/index.js

```jsx
import React from "react";
import ReactDOM from "react-dom";
import "./Modal.css";

function Modal({ children }) {
  return ReactDOM.createPortal(
    <div className="ModalBackground">{children}</div>,
    document.getElementById("modal")
  );
}

export { Modal };
```

2. Crear el estado en el contexto de la aplicacion

```jsx
...

function TodoProvider({ children }) {
  ....
  const [openModal, setOpenModal] = React.useState(true);
  ....
  return (
    <TodoContext.Provider value={{
      ....
      openModal,
      setOpenModal,
    }}>
      {children}
    </TodoContext.Provider>
  );
}

export { TodoContext, TodoProvider };
```

3. Modificar el archivo index.html

```html
<!DOCTYPE html>
<html lang="en">
  ....
  <body>
    ....
    <div id="root"></div>
    <div id="modal"></div>
    ....
  </body>
</html>
```

4. Modificar el archivo Modal.css

```css
.ModalBackground {
  background-color: rgba(32, 35, 41, 0.8);
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  position: fixed;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
}
```

5. Modificar el archivo AppUI.js

```jsx
....

function AppUI() {
  const {
    ....
    openModal,
    setOpenModal,
  } = React.useContext(TodoContext);

  return (
    <>
      ....
      <CreateTodoButton
        setOpenModal={setOpenModal}
      />

      {openModal && (
        <Modal>
          La funcionalidad de agregar TODO
        </Modal>
      )}
    </>
  );
}

export { AppUI };
```

6. Modificar el archivo CreateTodoButton.js

```jsx
import "./CreateTodoButton.css";

function CreateTodoButton({ setOpenModal }) {
  return (
    <button
      className="CreateTodoButton"
      onClick={() => {
        setOpenModal((state) => !state);
      }}
    >
      +
    </button>
  );
}

export { CreateTodoButton };
```

7. Modificar el archivo createTodoButton.css

```css
.CreateTodoButton {
  background-color: #61dafa;
  box-shadow: 0px 5px 25px rgba(97, 218, 250, 0.5);
  border: none;
  border-radius: 50%;
  cursor: pointer;
  font-size: 50px;
  position: fixed;
  bottom: 24px;
  right: 24px;
  font-weight: bold;
  color: #fafafa;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 64px;
  width: 64px;
  z-index: 1;

  transform: rotate(0);
  transition: 0.3s ease;
}

.CreateTodoButton:hover {
  transform: rotate(224deg);
}
```

## Formularios

1. Crear el componente TodoForm/index.js

```jsx
import React from "react";
import { TodoContext } from "../TodoContext";
import "./TodoForm.css";

function TodoForm() {
  const { addTodo, setOpenModal } = React.useContext(TodoContext);
  const [newTodoValue, setNewTodoValue] = React.useState("");

  const onSubmit = (event) => {
    event.preventDefault(); // Evita que se recargue la pagina
    addTodo(newTodoValue);
    setOpenModal(false);
  };

  const onCancel = () => {
    setOpenModal(false);
  };

  const onChange = (event) => {
    setNewTodoValue(event.target.value);
  };

  return (
    <form onSubmit={onSubmit}>
      <label>Escribe tu nuevo TODO</label>
      <textarea // input multilinea
        placeholder="Cortar cebolla para el almuerzo"
        value={newTodoValue}
        onChange={onChange}
      />
      <div className="TodoForm-buttonContainer">
        <button
          type="button"
          className="TodoForm-button TodoForm-button--cancel"
          onClick={onCancel}
        >
          Cancelar
        </button>
        <button type="submit" className="TodoForm-button TodoForm-button--add">
          Añadir
        </button>
      </div>
    </form>
  );
}

export { TodoForm };
```

2. Crear el componente TodoForm/TodoForm.css

```css
form {
  width: 90%;
  max-width: 300px;
  background-color: #fff;
  padding: 33px 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

label {
  text-align: center;
  font-weight: bold;
  font-size: 20px;
  color: #1e1e1f;
  margin-bottom: 26px;
}

textarea {
  background-color: #f9fbfc;
  border: 2px solid #202329;
  border-radius: 2px;
  box-shadow: 0px 5px 50px rgba(32, 35, 41, 0.25);
  color: #1e1e1f;
  font-size: 20px;
  text-align: center;
  padding: 12px;
  height: 96px;
  width: calc(100% - 25px);
}

textarea::placeholder {
  color: #a5a5a5;
  font-family: "Montserrat";
  font-weight: 400;
}

textarea:focus {
  outline-color: #61dafa;
}

.TodoForm-buttonContainer {
  margin-top: 14px;
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 100%;
}

.TodoForm-button {
  cursor: pointer;
  display: inline-block;
  font-size: 20px;
  color: #202329;
  font-weight: 400;
  width: 120px;
  height: 48px;
  border-radius: 2px;
  border: none;
  font-family: "Montserrat";
}

.TodoForm-button--add {
  background: #61dafa;
  box-shadow: 0px 5px 25px rgba(97, 218, 250, 0.5);
}

.TodoForm-button--cancel {
  background: transparent;
}
```

3. Modificar AppUI.js

```jsx
....

function AppUI() {
  ....

  return (
    <>
      ....
      {openModal && (
        <Modal>
          <TodoForm />
        </Modal>
      )}
    </>
  );
}

export { AppUI };
```

4. Modificar TodoContext.js

```jsx
....

const TodoContext = React.createContext();

function TodoProvider({ children }) {
  ....

  const addTodo = (text) => {
    const newTodos = [...todos];
    newTodos.push({
      text,
      completed: false,
    });
    saveTodos(newTodos);
  };

  ....
  return (

    <TodoContext.Provider value={{
      ....
      addTodo,
      completeTodo,
      deleteTodo,
      openModal,
      setOpenModal,
    }}>
      {children}
    </TodoContext.Provider>
  );
}

export { TodoContext, TodoProvider };
```

## Deploy de la aplicacion en github pages

1. En el archivo package.json modificar la propiedad Homepage para desplegar en github

```js
....
"homepage": "https://usuario_git_hub.github.io/nombre_del_repositorio/",
```

2. Instalar gh-pages

```bash
npm install --save-dev gh-pages
```

3. Crear un script en el archivo package.json

```js
....
"scripts": {
  ....
  "predeploy" : "npm run build",
  "deploy": "gh-pages -d build"
},
```

4. Ejecutar el script

```bash
npm run deploy
```

Si todo sale bien, deberia aparecer una nueva rama en el repositorio de github llamada gh-pages

5. En la configuracion del repositorio de github, en la seccion de GitHub Pages, seleccionar la rama gh-pages y la carpeta root
6. Finalmente, en la seccion de GitHub Pages, aparecera la url de la aplicacion

## Versiones de React

- En la package.json se puede ver la version de react que se esta utilizando

```js
....
"react": "^17.0.2",
```

Si cambias la version de react, debes ejecutar el siguiente comando

```bash
rm -rf node_modules
rm package-lock.json
npm install
```

Si tienes problemas, puedes buscar en la documentacion de react. Es importante saber adaptar a versiones anteriores de react, ya que es posible que en el futuro tengas que trabajar con proyectos que utilicen versiones anteriores de react.

## Creando proyectos de React

### create-react-app

```bash
npx create-react-app nombre_del_proyecto
```

### next.js

```bash
npm create-next-app@latest nombre_proyecto
```

# Modulo 4: Ecoomerce con React, Vite y Tailwind

## Enlaces de interes

1. [Repositorio Tienda en linea con React](https://github.com/platzi/curso-react-practico/tree/master)

## Vite

Vite es un nuevo compilador de código abierto que sirve para crear aplicaciones web
modernas con React, Vue, Svelte, Preact y TypeScript. Vite se centra en el
tiempo de compilación y el tiempo de ejecución rápido. No es un marco
completo, sino más bien un compilador de desarrollo que aprovecha las
importaciones nativas de ES Module para lograr un tiempo de compilación rápido
y un servidor de desarrollo instantáneo con recarga rápida.

Para crear un proyecto con Vite, debemos tener instalado Node.js y npm. Luego, abrimos una terminal y ejecutamos el siguiente comando:

```bash
npm create vite@latest
```

## Instalacion de TailwindCSS

[Documentacion](https://tailwindcss.com/docs/guides/vite)

**Nota**: Para empezar de cero un proyecto puedes eliminar la carpeta assets, limpiar el archivo App.css y el index.css y el App.jsx, debe quedar asi.

```jsx
import "./App.css";

function App() {
  return (
    <div className="bg-red-100">
      <h1>Hola Mundo</h1>
    </div>
  );
}

export default App;
```

## Paginas del ecommerce

Se crea una carpeta **Pages** donde se van a crear las paginas de la aplicacion. Estas paginas son App,Home, MyOrders, MyAccount, SingIn, MyOrder, NotFound.

_En la carpeta App debes trasladar todos los archivos referentes a App. Ten cuidado porque debes modificcar las importaciones en el archivo main.jsx_

Despues de crear las paginas debes importarlas en el archivo App/index.jsx

```jsx
import Home from "../Home";
import MyAccount from "../MyAccount";
import MyOrder from "../MyOrder";
import MyOrders from "../MyOrders";
import NotFound from "../NotFound";
import SignIn from "../SignIn";
import "./App.css";

const App = () => {
  return (
    <div className="bg-red-100">
      <Home />
      <MyAccount />
      <MyOrder />
      <MyOrders />
      <NotFound />
      <SignIn />
    </div>
  );
};

export default App;
```

## Enrutamiento con React Router Dom

1. Instalar react router dom

```bash
npm install react-router-dom
```

2. En App/index.jsx

```jsx
import { useRoutes, BrowserRouter } from 'react-router-dom'
....

const AppRoutes = () => {
  let routes = useRoutes([
    { path: '/', element: <Home /> },
    { path: '/my-account', element: <MyAccount /> },
    { path: '/my-order', element: <MyOrder /> },
    { path: '/my-orders', element: <MyOrders /> },
    { path: '/sign-in', element: <SignIn /> },
    { path: '/*', element: <NotFound /> },
  ])

  return routes
}

const App = () => {
  return (
    <BrowserRouter>
      <AppRoutes />
    </BrowserRouter>
  )
}

export default App
```

## Componente NavBar

1. Crear carpeta components y dentro de ella crear la carpeta NavBar/index.jsx
2. Componente [NavLink](https://reactrouter.com/en/main/components/nav-link)

**Explicacion de algunas partes del codigo**

```jsx
<NavLink
  to="/"
  className={({ isActive }) => (isActive ? activeStyle : undefined)}
>
  All
</NavLink>
```

NavLink es un componente que nos permite crear links en nuestra aplicacion. El atributo `to` es el destino del link. El atributo isActive es una funcion que nos permite agregar estilos cuando el link esta activo.

**Clases nuevas de Tailwind**

- _Gap_: Nos permite agregar un espacio entre los elementos de un contenedor.

[Documentacion](https://tailwindcss.com/docs/gap)

- _underline_: Nos permite agregar una linea debajo del texto.

- _underline-offset_: Nos permite agregar un espacio entre el texto y la linea.

```jsx
import { NavLink } from "react-router-dom";

const Navbar = () => {
  const activeStyle = "underline underline-offset-4"; // Estilo para cuando el link esta activo

  return (
    <nav className="flex justify-between items-center fixed z-10 w-full py-5 px-8 text-sm font-light">
      <ul className="flex items-center gap-3">
        <li className="font-semibold text-lg">
          <NavLink to="/">Shopi</NavLink>
        </li>
        <li>
          <NavLink
            to="/"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            All
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/clothes"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            Clothes
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/electronics"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            Electronics
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/furnitures"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            Furnitures
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/toys"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            Toys
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/others"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            Others
          </NavLink>
        </li>
      </ul>
      <ul className="flex items-center gap-3">
        <li className="text-black/60">teff@platzi.com</li>
        <li>
          <NavLink
            to="/my-orders"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            My Orders
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/my-account"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            My Account
          </NavLink>
        </li>
        <li>
          <NavLink
            to="/sing-in"
            className={({ isActive }) => (isActive ? activeStyle : undefined)}
          >
            Sign In
          </NavLink>
        </li>
        <li>🛒 0</li>
      </ul>
    </nav>
  );
};

export default Navbar;
```

1. En App/index.jsx

```jsx
....
import Navbar from '../../Components/Navbar'
import './App.css'

const AppRoutes = () => {
  let routes = useRoutes([
    { path: '/', element: <Home /> },
    { path: '/my-account', element: <MyAccount /> },
    { path: '/my-order', element: <MyOrder /> },
    { path: '/my-orders', element: <MyOrders /> },
    { path: '/sign-in', element: <SignIn /> },
    { path: '/*', element: <NotFound /> },
  ])

  return routes
}

const App = () => {
  return (
    <BrowserRouter>
      <AppRoutes />
      <Navbar />
    </BrowserRouter>
  )
}

export default App
```

## Componente Layout

1. Crear carpeta Layout y dentro de ella crear el archivo index.jsx
2. En el archivo index.jsx

```jsx
const Layout = ({ children }) => {
  return <div className="flex flex-col items-center mt-20">{children}</div>;
};

export default Layout;
```

3. En Home/index.jsx

```jsx
import Layout from "../../Components/Layout";

function Home() {
  return <Layout>Home</Layout>;
}

export default Home;
```

4. Replicar lo mismo en las demas paginas.

## Componente Card

1. Crear carpeta Components/Card y dentro de ella crear el archivo index.jsx

**Clases de tailwind nuevas**

- _cursor-pointer_: Nos permite cambiar el cursor del mouse cuando pasamos por encima de un elemento.
- _object-cover_: Nos permite ajustar la imagen al tamaño del contenedor. [Documentacion](https://tailwindcss.com/docs/object-fit#basic-usage)

```jsx
const Card = () => {
  return (
    <div className="bg-white cursor-pointer w-56 h-60 rounded-lg">
      <figure className="relative mb-2 w-full h-4/5">
        <span className="absolute bottom-0 left-0 bg-white/60 rounded-lg text-black text-xs m-2 px-3 py-0.5">
          Electronics
        </span>
        <img
          className="w-full h-full object-cover rounded-lg"
          src="https://images.pexels.com/photos/1037992/pexels-photo-1037992.jpeg?auto=compress&cs=tinysrgb&w=1260&h=750&dpr=1"
          alt="headphones"
        />
        <div className="absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1">
          +
        </div>
      </figure>
      <p className="flex justify-between">
        <span className="text-sm font-light">Headphones</span>
        <span className="text-lg font-medium">$300</span>
      </p>
    </div>
  );
};

export default Card;
```

## Consumiendo una API

[API](https://fakeapi.platzi.com/)

1. En Home/index.jsx

**Explicacion de algunas partes del codigo**

- _fetch_: Nos permite hacer peticiones a una API.La estructura de la peticion es la siguiente:

```jsx
fetch("url de la api")
  .then((response) => response.json())
  .then((data) => console.log(data));
```

o tambien puedes hacerlo de la siguiente manera:

```jsx
const response = await fetch("url de la api");
const data = await response.json();
console.log(data);
```

- _map_: Nos permite recorrer un arreglo y retornar un nuevo arreglo con los elementos que necesitamos. La estructura es la siguiente:

```jsx
const array = [1, 2, 3, 4, 5];
const newArray = array.map((item) => item * 2);
console.log(newArray); // [2,4,6,8,10]
```

En este caso, vamos a recorrer los items, si estos existen. Vamos a crear un componente Card por cada item que se tenga (React nos dice que por cada elementos debemos tener un id).

_Cuando trabajamos con lambda function podemos tener un return de dos maneras: la primera es cuando tenemos una sola linea de codigo y la segunda es cuando tenemos mas de una linea de codigo._

```jsx
const array = [1, 2, 3, 4, 5];
const newArray = array.map((item) => item * 2);
console.log(newArray); // [2,4,6,8,10]
```

```jsx
const array = [1, 2, 3, 4, 5];
const newArray = array.map((item) => {
  const newItem = item * 2;
  return newItem;
});
console.log(newArray); // [2,4,6,8,10]
```

**Clases de tailwind nuevas**

- _grid-col_: Nos permite definir el numero de columnas que va a tener un contenedor. [Documentacion](https://tailwindcss.com/docs/grid-template-columns)
- max-w-screen-lg: Nos permite definir el ancho maximo de un contenedor. [Documentacion](https://tailwindcss.com/docs/max-width)

```jsx
import { useState, useEffect } from "react";
import Layout from "../../Components/Layout";
import Card from "../../Components/Card";

const Home = () => {
  const [items, setItems] = useState(null);

  useEffect(() => {
    fetch("https://api.escuelajs.co/api/v1/products")
      .then((response) => response.json())
      .then((data) => setItems(data));
  }, []);

  return (
    <Layout>
      Home
      <div className="grid gap-4 grid-cols-4 w-full max-w-screen-lg">
        {items?.map((item) => (
          <Card key={item.id} data={item} />
        ))}
      </div>
    </Layout>
  );
};

export default Home;
```

2. En Card/index.jsx

```jsx
const Card = (data) => {
  return (
    <div className="bg-white cursor-pointer w-56 h-60 rounded-lg">
      <figure className="relative mb-2 w-full h-4/5">
        <span className="absolute bottom-0 left-0 bg-white/60 rounded-lg text-black text-xs m-2 px-3 py-0.5">
          {data.data.category.name}
        </span>
        <img
          className="w-full h-full object-cover rounded-lg"
          src={data.data.images[0]}
          alt={data.data.title}
        />
        <div className="absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1">
          +
        </div>
      </figure>
      <p className="flex justify-between">
        <span className="text-sm font-light">{data.data.title}</span>
        <span className="text-lg font-medium">${data.data.price}</span>
      </p>
    </div>
  );
};

export default Card;
```

## Contexto global de la aplicacion

1. Crear la carpeta src/Context y dentro de ella crear el archivo index.jsx

**Explicacion de algunas partes del codigo**

```jsx
import { createContext } from "react";

const ShoppingCartContext = createContext();

export const ShoppingCartProvider = ({ children }) => {
  return (
    <ShoppingCartContext.Provider>{children}</ShoppingCartContext.Provider>
  );
};
```

2. En App/index.jsx

```jsx
....
import { ShoppingCartProvider } from '../../Context'
....

const App = () => {
  return (
    <BrowserRouter>
      <ShoppingCartProvider>
        <AppRoutes />
        <Navbar />
      </ShoppingCartProvider>
    </BrowserRouter>
  )
}

export default App
```

## Contador de productos en el carrito

1. En Context/index.jsx

```jsx
import { createContext, useState } from "react";

export const ShoppingCartContext = createContext();

export const ShoppingCartProvider = ({ children }) => {
  const [count, setCount] = useState(0);

  return (
    <ShoppingCartContext.Provider
      value={{
        count,
        setCount,
      }}
    >
      {children}
    </ShoppingCartContext.Provider>
  );
};
```

2. En Card/index.jsx

```jsx
import { useContext } from "react";
import { ShoppingCartContext } from "../../Context";

const Card = (data) => {
  const context = useContext(ShoppingCartContext);

  return (
    <div className="bg-white cursor-pointer w-56 h-60 rounded-lg">
      ....
      <div
        className="absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1"
        onClick={() => context.setCount(context.count + 1)}
      >
        +
      </div>
      ....
    </div>
  );
};

export default Card;
```

3. En Navbar/index.jsx

```jsx
import { useContext } from 'react'
import { NavLink } from 'react-router-dom'
import { ShoppingCartContext } from '../../Context'

const Navbar = () => {
  const context = useContext(ShoppingCartContext)
  ....

  return (
    <nav className='flex justify-between items-center fixed z-10 top-0 w-full py-5 px-8 text-sm font-light'>
      ....
      <ul className='flex items-center gap-3'>
        ....
        <li>
          🛒 {context.count}
        </li>
      </ul>
    </nav>
  )
}

export default Navbar
```

## Abriendo el detalle de cada producto

### Maquetacion e iconos

1. Crear Componets/ProductDetail y dentro de ella crear el archivo index.jsx

**Explicacion de algunas partes del codigo**

- _aside_: Nos permite crear un contenedor que se va a ubicar en el lado derecho de la pantalla.
- _height: calc(100vh - 68px)_: Nos permite definir el alto del contenedor. En este caso, el alto va a ser el 100% de la pantalla menos 68px. 68px corresponde al alto de la barra de navegacion. Esta funcionalidad permite que no haya un scroll en la pagina.

**Clases nuevas de tailwind**

_Puedes utilizar clases de CSS junto con Tailwind_

2. Crear ProductDetail/styles.css

```css
.product-detail {
  width: 360px;
  height: calc(100vh - 68px);
  top: 68px;
}
```

3. Puedes utilizar la libreria heroicons para agregar iconos a tu aplicacion. [Documentacion](https://heroicons.com/)

```jsx
import { XMarkIcon } from "@heroicons/react/24/solid";
import "./styles.css";

const ProductDetail = () => {
  return (
    <aside className="product-detail flex flex-col fixed right-0 border border-black rounded-lg bg-white">
      <div className="flex justify-between items-center p-6">
        <h2 className="font-medium text-xl">Detail</h2>
        <div>
          <XMarkIcon className="h-6 w-6 text-black"></XMarkIcon>
        </div>
      </div>
    </aside>
  );
};

export default ProductDetail;
```

3. En Home/index.jsx

```jsx
....
import ProductDetail from '../../Components/ProductDetail'

function Home() {
  ....

  return (
    <Layout>
      Home
      <div className='grid gap-4 grid-cols-4 w-full max-w-screen-lg'>
        {
          items?.map(item => (
            <Card key={item.id} data={item} />
          ))
        }
      </div>
      <ProductDetail />
    </Layout>
  )
}

export default Home
```

4. En Navbar/index.jsx

```jsx
....
import { ShoppingBagIcon } from '@heroicons/react/24/solid'
import { ShoppingCartContext } from '../../Context'

const Navbar = () => {
  ....
  return (
    <nav className='flex justify-between items-center fixed z-10 top-0 w-full py-5 px-8 text-sm font-light'>
      <ul className='flex items-center gap-3'>
        ....
        <li className='flex items-center'>
          <ShoppingBagIcon className='h-6 w-6 text-black'></ShoppingBagIcon>
          <div>{context.count}</div>
        </li>
      </ul>
    </nav>
  )
}

export default Navbar
```

5. en Card/index.jsx

```jsx
....
import { PlusIcon } from '@heroicons/react/24/solid'
import { ShoppingCartContext } from '../../Context'

const Card = (data) => {
  ....
  return (
    <div className='bg-white cursor-pointer w-56 h-60 rounded-lg'>
      <figure className='relative mb-2 w-full h-4/5'>
        ....
        <div
          className='absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1'
          onClick={() => context.setCount(context.count + 1)}>
          <PlusIcon className='h-6 w-6 text-black'></PlusIcon>
        </div>
      </figure>
      ....
    </div>
  )
}

export default Card
```

### Logica del componente

1. En Context/index.jsx

```jsx
....

export const ShoppingCartProvider = ({children}) => {
  // Shopping Cart · Increment quantity
  const [count, setCount] = useState(0)

  // Product Detail · Open/Close
  const [isProductDetailOpen, setIsProductDetailOpen] = useState(false)
  const openProductDetail = () => setIsProductDetailOpen(true)
  const closeProductDetail = () => setIsProductDetailOpen(false)

  // Product Detail · Show product
  const [productToShow, setProductToShow] = useState({})

  return (
    <ShoppingCartContext.Provider value={{
      count,
      setCount,
      openProductDetail,
      closeProductDetail,
      isProductDetailOpen,
      productToShow,
      setProductToShow
    }}>
      {children}
    </ShoppingCartContext.Provider>
  )
}
```

2. En Card/index.jsx

```jsx
....

const Card = (data) => {
....

  const showProduct = (productDetail) => {
    context.openProductDetail()
    context.setProductToShow(productDetail)
  }

  return (
    <div
      className='bg-white cursor-pointer w-56 h-60 rounded-lg'
      onClick={() => showProduct(data.data)}>
      ....
    </div>
  )
}

export default Card
```

3. En ProductDetail/index.jsx

```jsx
....
import { ShoppingCartContext } from '../../Context'
import './styles.css'

const ProductDetail = () => {
  ....
  return (
    <aside
      className={`${context.isProductDetailOpen ? 'flex' : 'hidden'} product-detail flex-col fixed right-0 border border-black rounded-lg bg-white`}>
      <div className='flex justify-between items-center p-6'>
        <h2 className='font-medium text-xl'>Detail</h2>
        <div>
          <XMarkIcon
            className='h-6 w-6 text-black cursor-pointer'
            onClick={() => context.closeProductDetail()}></XMarkIcon>
        </div>
      </div>
      <figure className='px-6'>
        <img
          className='w-full h-full rounded-lg'
          src={context.productToShow.images[0]}
          alt={context.productToShow.title} />
      </figure>
      <p className='flex flex-col p-6'>
        <span className='font-medium text-2xl mb-2'>${context.productToShow.price}</span>
        <span className='font-medium text-md'>${context.productToShow.title}</span>
        <span className='font-light text-sm'>${context.productToShow.description}</span>
      </p>
    </aside>
  )
}

export default ProductDetail
```

## Agregando el carrito de compras

1. Vamos a crear la funcionalidad de llevar productos a un carrito de compras

En Context/index.jsx

```jsx
....

export const ShoppingCartProvider = ({children}) => {
  ....
  // Checkout Side Menu · Open/Close
  const [isCheckoutSideMenuOpen, setIsCheckoutSideMenuOpen] = useState(false)
  const openCheckoutSideMenu = () => setIsCheckoutSideMenuOpen(true)
  const closeCheckoutSideMenu = () => setIsCheckoutSideMenuOpen(false)

  // Shopping Cart · Add products to cart
  const [cartProducts, setCartProducts] = useState([])


  return (
    <ShoppingCartContext.Provider value={{
      ....
      cartProducts,
      setCartProducts,
      isCheckoutSideMenuOpen,
      openCheckoutSideMenu,
      closeCheckoutSideMenu
    }}>
      {children}
    </ShoppingCartContext.Provider>
  )
}
```

2. En Card/index.jsx

```jsx
....

const Card = (data) => {
  ....

  const addProductsToCart = (productData) => {
    context.setCount(context.count + 1)
    context.setCartProducts([...context.cartProducts, productData])
    console.log('CART: ', context.cartProducts)
  }

  return (
    <div
      className='bg-white cursor-pointer w-56 h-60 rounded-lg'
      onClick={() => showProduct(data.data)}>
      <figure className='relative mb-2 w-full h-4/5'>
        ....
        <div
          className='absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1'
          onClick={() => addProductsToCart(data.data)}>
          <PlusIcon className='h-6 w-6 text-black'></PlusIcon>
        </div>
      </figure>
    </div>
  )
}

export default Card
```

### SlideMenu del carrito de compras

1. En Components/SlideMenu y dentro de ella crear el archivo index.jsx

```jsx
import { useContext } from "react";
import { XMarkIcon } from "@heroicons/react/24/solid";
import { ShoppingCartContext } from "../../Context";
import "./styles.css";

const CheckoutSideMenu = () => {
  const context = useContext(ShoppingCartContext);

  return (
    <aside
      className={`${
        context.isCheckoutSideMenuOpen ? "flex" : "hidden"
      } checkout-side-menu flex-col fixed right-0 border border-black rounded-lg bg-white`}
    >
      <div className="flex justify-between items-center p-6">
        <h2 className="font-medium text-xl">My Order</h2>
        <div>
          <XMarkIcon
            className="h-6 w-6 text-black cursor-pointer"
            onClick={() => context.closeCheckoutSideMenu()}
          ></XMarkIcon>
        </div>
      </div>
    </aside>
  );
};

export default CheckoutSideMenu;
```

2. en SlideMenu/styles.css

```css
.checkout-side-menu {
  width: 360px;
  height: calc(100vh - 68px);
  top: 68px;
}
```

3. En Card/index.jsx

```jsx
....

const Card = (data) => {
  ....

  const addProductsToCart = (event, productData) => {
    event.stopPropagation() // Evita que se propague el evento, es decir, que no se ejecute el evento del padre
    context.setCount(context.count + 1)
    context.setCartProducts([...context.cartProducts, productData])
    context.openCheckoutSideMenu()
    context.closeProductDetail()
    console.log('CART: ', context.cartProducts)
  }

  return (
    <div
      className='bg-white cursor-pointer w-56 h-60 rounded-lg'
      onClick={() => showProduct(data.data)}>
      <figure className='relative mb-2 w-full h-4/5'>
        <div
          className='absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1'
          onClick={(event) => addProductsToCart(event, data.data)}>
          <PlusIcon className='h-6 w-6 text-black'></PlusIcon>
        </div>
      </figure>
      ....
    </div>
  )
}

export default Card
```

4. En App/index.jsx. Para que el carrito pueda abrirse desde cualquier parte de la aplicacion

```jsx
....
import CheckoutSideMenu from '../../Components/CheckoutSideMenu'
import './App.css'

....

const App = () => {
  return (
    <ShoppingCartProvider>
      <BrowserRouter>
        ....
        <CheckoutSideMenu />
      </BrowserRouter>
    </ShoppingCartProvider>
  )
}

export default App
```

## Componente OrderCard

1. En Components/OrderCard y dentro de ella crear el archivo index.jsx

```jsx
import { XMarkIcon } from "@heroicons/react/24/solid";

const OrderCard = (props) => {
  const { title, imageUrl, price } = props;

  return (
    <div className="flex justify-between items-center mb-3">
      <div className="flex items-center gap-2">
        <figure className="w-20 h-20">
          <img
            className="w-full h-full rounded-lg object-cover"
            src={imageUrl}
            alt={title}
          />
        </figure>
        <p className="text-sm font-light">{title}</p>
      </div>
      <div className="flex items-center gap-2">
        <p className="text-lg font-medium">{price}</p>
        <XMarkIcon className="h-6 w-6 text-black cursor-pointer"></XMarkIcon>
      </div>
    </div>
  );
};

export default OrderCard;
```

2. En CheckoutSideMenu/index.jsx

```jsx
....
import OrderCard from '../../Components/OrderCard'
import './styles.css'

const CheckoutSideMenu = () => {
  ....

  return (
    <aside
      className={`${context.isCheckoutSideMenuOpen ? 'flex' : 'hidden'} checkout-side-menu flex-col fixed right-0 border border-black rounded-lg bg-white`}>
      <div className='px-6 overflow-y-scroll'>
        {
          context.cartProducts.map(product => (
            <OrderCard
              key={product.id}
              title={product.title}
              imageUrl={product.images}
              price={product.price}
            />
          ))
        }
      </div>
    </aside>
  )
}

export default CheckoutSideMenu
```

### Evitando duplicados en el carrito de compras

1. En Card/index.jsx

```jsx
import { useContext } from 'react'
import { PlusIcon, CheckIcon } from '@heroicons/react/24/solid'
import { ShoppingCartContext } from '../../Context'

const Card = (data) => {
  ....
  const renderIcon = (id) => {
    const isInCart = context.cartProducts.filter(product => product.id === id).length > 0

    if (isInCart) {
      return (
        <div
          className='absolute top-0 right-0 flex justify-center items-center bg-black w-6 h-6 rounded-full m-2 p-1'>
          <CheckIcon className='h-6 w-6 text-white'></CheckIcon>
        </div>
      )
    } else {
      return (
        <div
          className='absolute top-0 right-0 flex justify-center items-center bg-white w-6 h-6 rounded-full m-2 p-1'
          onClick={(event) => addProductsToCart(event, data.data)}>
          <PlusIcon className='h-6 w-6 text-black'></PlusIcon>
        </div>
      )
    }
  }

  return (
    <div
      className='bg-white cursor-pointer w-56 h-60 rounded-lg'
      onClick={() => showProduct(data.data)}>
      <figure className='relative mb-2 w-full h-4/5'>
        <span className='absolute bottom-0 left-0 bg-white/60 rounded-lg text-black text-xs m-2 px-3 py-0.5'>{data.data.category.name}</span>
        <img className='w-full h-full object-cover rounded-lg' src={data.data.images[0]} alt={data.data.title} />
        {renderIcon(data.data.id)}
      </figure>
      <p className='flex justify-between'>
        <span className='text-sm font-light'>{data.data.title}</span>
        <span className='text-lg font-medium'>${data.data.price}</span>
      </p>
    </div>
  )
}

export default Card
```

### Eliminar productos del carrito

1. En Components/OrderCard/index.jsx

```jsx
....

const OrderCard = props => {
  const { id, title, imageUrl, price, handleDelete } = props

  return (
    <div className="flex justify-between items-center mb-3">
      ....
      <div className='flex items-center gap-2'>
        <p className='text-lg font-medium'>{price}</p>
        <XMarkIcon onClick={() => handleDelete(id)} className='h-6 w-6 text-black cursor-pointer'></XMarkIcon>
      </div>
    </div>
  )
}

export default OrderCard
```

2. En CheckoutSideMenu/index.jsx

```jsx
....

const CheckoutSideMenu = () => {
  ....
  const handleDelete = (id) => {
    const filteredProducts = context.cartProducts.filter(product => product.id != id)
    context.setCartProducts(filteredProducts)
  }

  return (
    <aside
      className={`${context.isCheckoutSideMenuOpen ? 'flex' : 'hidden'} checkout-side-menu flex-col fixed right-0 border border-black rounded-lg bg-white`}>
      ....
      <div className='px-6 overflow-y-scroll'>
        {
          context.cartProducts.map(product => (
            <OrderCard
              key={product.id}
              id={product.id}
              title={product.title}
              imageUrl={product.images}
              price={product.price}
              handleDelete={handleDelete}
            />
          ))
        }
      </div>
    </aside>
  )
}

export default CheckoutSideMenu
```

### Total de la compra

1. En utils/index.js

```js
/**
 * This function calculates total price of a new order
 * @param {Array} products cartProduct: Array of Objects
 * @returns {numer} Total price
 */

// Lo anterior es un comentario de la funcion
export const totalPrice = (products) => {
  let sum = 0;
  products.forEach((product) => (sum += product.price));
  return sum;
};
```

2. En CheckoutSideMenu/index.jsx

```jsx
....
import { totalPrice } from '../../utils'
import './styles.css'

const CheckoutSideMenu = () => {
  ....

  return (
    <aside
      className={`${context.isCheckoutSideMenuOpen ? 'flex' : 'hidden'} checkout-side-menu flex-col fixed right-0 border border-black rounded-lg bg-white`}>

      <div className='px-6'>
        <p className='flex justify-between items-center'>
          <span className='font-light'>Total:</span>
          <span className='font-medium text-2xl'>${totalPrice(context.cartProducts)}</span>
        </p>
      </div>
    </aside>
  )
}

export default CheckoutSideMenu
```

## Pagina MyOrders

1. En Context/index.jsx

```jsx
....

export const ShoppingCartProvider = ({children}) => {
  ....
  const [order, setOrder] = useState([])

  return (
    <ShoppingCartContext.Provider value={{
      ....
      order,
      setOrder
    }}>
      {children}
    </ShoppingCartContext.Provider>
  )
}
```

2. En CheckoutSideMenu/index.jsx

```jsx
import {Link} from 'react-router-dom'
....

const CheckoutSideMenu = () => {
  ....

  const handleCheckout = () => {
    const orderToAdd = {
      date: '01.02.23',
      products: context.cartProducts,
      totalProducts: context.cartProducts.length,
      totalPrice: totalPrice(context.cartProducts)
    }

    context.setOrder([...context.order, orderToAdd])
    context.setCartProducts([])
  }

  return (
    <aside
      className={`${context.isCheckoutSideMenuOpen ? 'flex' : 'hidden'} checkout-side-menu flex-col fixed right-0 border border-black rounded-lg bg-white`}>
      ....
      <div className='px-6 overflow-y-scroll flex-1'>
        {
          context.cartProducts.map(product => (
            <OrderCard
              key={product.id}
              id={product.id}
              title={product.title}
              imageUrl={product.images}
              price={product.price}
              handleDelete={handleDelete}
            />
          ))
        }
      </div>
      <div className='px-6 mb-6'>
        <p className='flex justify-between items-center mb-2'>
          <span className='font-light'>Total:</span>
          <span className='font-medium text-2xl'>${totalPrice(context.cartProducts)}</span>
        </p>
        <Link to='my-orders/last'>
        <button className='bg-black py-3 text-white w-full rounded-lg' onClick={() => handleCheckout()}>Checkout</button>
      </div>
    </aside>
  )
}

export default CheckoutSideMenu
```

3. en App/index.jsx

```jsx
....

const AppRoutes = () => {
  let routes = useRoutes([
    ....
    { path: '/my-orders/last', element: <MyOrder /> },
    ....
  ])
  return routes
}

const App = () => {
  return (
    ....
  )
}

export default App
```

4. En MyOrder/index.jsx

```jsx
import { useContext } from "react";
import { ShoppingCartContext } from "../../Context";
import Layout from "../../Components/Layout";
import OrderCard from "../../Components/OrderCard";

function MyOrder() {
  const context = useContext(ShoppingCartContext);

  return (
    <Layout>
      MyOrder
      <div className="flex flex-col w-80">
        {context.order?.slice(-1)[0].products.map((product) => (
          <OrderCard
            key={product.id}
            id={product.id}
            title={product.title}
            imageUrl={product.images}
            price={product.price}
          />
        ))}
      </div>
    </Layout>
  );
}

export default MyOrder;
```

5. En OrderCard/index.jsx

```jsx
....

const OrderCard = props => {
  const { id, title, imageUrl, price, handleDelete } = props

  let renderXMarkIcon
  if (handleDelete) {
    renderXMarkIcon = <XMarkIcon onClick={() => handleDelete(id)} className='h-6 w-6 text-black cursor-pointer'></XMarkIcon>
  }

  return (
    <div className="flex justify-between items-center mb-3">
     ....
      <div className='flex items-center gap-2'>
        <p className='text-lg font-medium'>{price}</p>
        {renderXMarkIcon}
      </div>
    </div>
  )
}

export default OrderCard
```

## Pagina MyOrders

1. En Components/OrdersCard/index.jsx

```jsx
import { XMarkIcon } from "@heroicons/react/24/solid";

const OrdersCard = (props) => {
  const { totalPrice, totalProducts } = props;

  return (
    <div className="flex justify-between items-center mb-3 border border-black">
      <p>
        <span>01.02.23</span>
        <span>{totalProducts}</span>
        <span>{totalPrice}</span>
      </p>
    </div>
  );
};

export default OrdersCard;
```

2. En Pages/MyOrders/index.jsx

```jsx
import { useContext } from "react";
import { Link } from "react-router-dom";
import Layout from "../../Components/Layout";
import { ShoppingCartContext } from "../../Context";
import OrdersCard from "../../Components/OrdersCard";

function MyOrders() {
  const context = useContext(ShoppingCartContext);

  return (
    <Layout>
      <div className="flex items-center justify-center relative w-80">
        <h1>My Orders</h1>
      </div>
      {context.order.map((order, index) => (
        <Link key={index} to={`/my-orders/${index}`}>
          <OrdersCard
            totalPrice={order.totalPrice}
            totalProducts={order.totalProducts}
          />
        </Link>
      ))}
    </Layout>
  );
}

export default MyOrders;
```

3. En Pages/MyOrder/index.jsx

```jsx
import { useContext } from 'react'
import { Link } from 'react-router-dom'
import { ChevronLeftIcon } from '@heroicons/react/24/solid'
....

function MyOrder() {
  ....

  return (
    <Layout>
      <div className='flex items-center justify-center relative w-80 mb-6'>
        <Link to='/my-orders' className='absolute left-0'>
          <ChevronLeftIcon className='h-6 w-6 text-black cursor-pointer' />
        </Link>
        <h1>My Order</h1>
      </div>
      ....
    </Layout>
  )
}

export default MyOrder
```

4. En MyOrder/index.jsx

```jsx
....

function MyOrder() {
  ....
  const currentPath = window.location.pathname
  let index = currentPath.substring(currentPath.lastIndexOf('/') + 1)
  if (index === 'last') index = context.order?.length - 1

  return (
    <Layout>
      ....
      <div className='flex flex-col w-80'>
        {
          context.order?.[index]?.products.map(product => (
            <OrderCard
              key={product.id}
              id={product.id}
              title={product.title}
              imageUrl={product.images}
              price={product.price}
            />
          ))
        }
      </div>
    </Layout>
  )
}

export default MyOrder
```

5. En App/index.jsx

```jsx
....

const AppRoutes = () => {
  let routes = useRoutes([
    ....
    { path: '/my-orders', element: <MyOrders /> },
    { path: '/my-orders/last', element: <MyOrder /> },
    { path: '/my-orders/:id', element: <MyOrder /> },
    ....
  ])

  return routes
}
....
```

6. En OrdersCard/index.jsx

```jsx
....

const OrdersCard = props => {
  ....
  return (
    <div className="flex justify-between items-center mb-3 border border-black rounded-lg p-4 w-80">
      <div className='flex justify-between w-full'>
        <p className='flex flex-col'>
          <span className='font-light'>01.02.23</span>
          <span className='font-light'>{totalProducts} articles</span>
        </p>
        <p className='flex items-center gap-2'>
          <span className='font-medium text-2xl'>${totalPrice}</span>
          <ChevronRightIcon className='h-6 w-6 text-black cursor-pointer' />
        </p>
      </div>
    </div>
  )
}

export default OrdersCard
```

## Buscados de productos

1. En Context/index.jsx

```jsx
import { createContext, useState, useEffect } from 'react'

...

export const ShoppingCartProvider = ({children}) => {
  ....
  // Get products
  const [items, setItems] = useState(null)

  // Get products by title
  const [searchByTitle, setSearchByTitle] = useState(null)
  console.log('searchByTitle: ', searchByTitle)

  useEffect(() => {
    fetch('https://api.escuelajs.co/api/v1/products')
      .then(response => response.json())
      .then(data => setItems(data))
  }, [])

  return (
    <ShoppingCartContext.Provider value={{
      ....
      items,
      setItems,
      searchByTitle,
      setSearchByTitle
    }}>
      {children}
    </ShoppingCartContext.Provider>
  )
}
```

2. En Home/index.jsx

```jsx
import { useContext } from 'react'
....

function Home() {
  ....
  return (
    <Layout>
      <div className='flex items-center justify-center relative w-80 mb-4'>
        <h1 className='font-medium text-xl'>Exclusive Products</h1>
      </div>
      <input
        type="text"
        placeholder='Search a product'
        className='rounded-lg border border-black w-80 p-4 mb-4 focus:outline-none'
        onChange={(event) => context.setSearchByTitle(event.target.value)} />
      ....
      <ProductDetail />
    </Layout>
  )
}

export default Home
```

4. En Context/index.jsx

```jsx
....

export const ShoppingCartProvider = ({children}) => {
  ....
  const [filteredItems, setFilteredItems] = useState(null)

  // Get products by title
  const [searchByTitle, setSearchByTitle] = useState(null)

  useEffect(() => {
    fetch('https://api.escuelajs.co/api/v1/products')
      .then(response => response.json())
      .then(data => setItems(data))
  }, [])

  const filteredItemsByTitle = (items, searchByTitle) => {
    return items?.filter(item => item.title.toLowerCase().includes(searchByTitle.toLowerCase()))
  }

  useEffect(() => {
    if (searchByTitle) setFilteredItems(filteredItemsByTitle(items, searchByTitle))
  }, [items, searchByTitle])

  return (
    <ShoppingCartContext.Provider value={{
      ...
      searchByTitle,
      setSearchByTitle,
      filteredItems
    }}>
      {children}
    </ShoppingCartContext.Provider>
  )
}
```

3. En Home/index.jsx

```jsx
....

function Home() {
  ....

  const renderView = () => {
    if (context.searchByTitle?.length > 0) {
      if (context.filteredItems?.length > 0) {
        return (
          context.filteredItems?.map(item => (
            <Card key={item.id} data={item} />
          ))
        )
      } else {
        return (
          <div>We don't have anything :(</div>
        )
      }
    } else {
      return (
        context.items?.map(item => (
          <Card key={item.id} data={item} />
        ))
      )
    }
  }

  return (
    <Layout>
      ....
      <div className='grid gap-4 grid-cols-4 w-full max-w-screen-lg'>
        {renderView()}
      </div>
      <ProductDetail />
    </Layout>
  )
}

export default Home
```

## Filtrando por categorias

1. En App/index.jsx

```jsx
....

const AppRoutes = () => {
  let routes = useRoutes([
    { path: '/', element: <Home /> },
    { path: '/clothes', element: <Home /> },
    { path: '/electronics', element: <Home /> },
    { path: '/furnitures', element: <Home /> },
    { path: '/toys', element: <Home /> },
    { path: '/othes', element: <Home /> },
    ....
  ])
  return routes
}
....
```

2. En Navbar/index.jsx

```jsx
....
import { ShoppingCartContext } from '../../Context'

const Navbar = () => {
  const context = useContext(ShoppingCartContext)
  ....

  return (
    <nav className='flex justify-between items-center fixed z-10 top-0 w-full py-5 px-8 text-sm font-light'>
      <ul className='flex items-center gap-3'>
        ....
        <li>
          <NavLink
            to='/'
            onClick={() => context.setSearchByCategory()}
            className={({ isActive }) =>
              isActive ? activeStyle : undefined
            }>
            All
          </NavLink>
        </li>
        <li>
          <NavLink
            to='/clothes'
            onClick={() => context.setSearchByCategory('clothes')}
            className={({ isActive }) =>
              isActive ? activeStyle : undefined
            }>
            Clothes
          </NavLink>
        </li>
        <li>
          <NavLink
            to='/electronics'
            onClick={() => context.setSearchByCategory('electronics')}
            className={({ isActive }) =>
              isActive ? activeStyle : undefined
            }>
            Electronics
          </NavLink>
        </li>
        <li>
          <NavLink
            to='/furnitures'
            onClick={() => context.setSearchByCategory('furnitures')}
            className={({ isActive }) =>
              isActive ? activeStyle : undefined
            }>
            Furnitures
          </NavLink>
        </li>
        <li>
          <NavLink
            to='/toys'
            onClick={() => context.setSearchByCategory('toys')}
            className={({ isActive }) =>
              isActive ? activeStyle : undefined
            }>
            Toys
          </NavLink>
        </li>
        <li>
          <NavLink
            to='/others'
            onClick={() => context.setSearchByCategory('others')}
            className={({ isActive }) =>
              isActive ? activeStyle : undefined
            }>
            Others
          </NavLink>
        </li>
      </ul>
      ....
    </nav>
  )
}

export default Navbar
```

3. En Context/index.jsx

```jsx
....

export const ShoppingCartProvider = ({children}) => {
  // Get products by category
  const [searchByCategory, setSearchByCategory] = useState(null)

  ....

  const filteredItemsByCategory = (items, searchByCategory) => {
    return items?.filter(item => item.category.name.toLowerCase().includes(searchByCategory.toLowerCase()))
  }

  const filterBy = (searchType, items, searchByTitle, searchByCategory) => {
    if (searchType === 'BY_TITLE') {
      return filteredItemsByTitle(items, searchByTitle)
    }

    if (searchType === 'BY_CATEGORY') {
      return filteredItemsByCategory(items, searchByCategory)
    }

    if (searchType === 'BY_TITLE_AND_CATEGORY') {
      return filteredItemsByCategory(items, searchByCategory).filter(item => item.title.toLowerCase().includes(searchByTitle.toLowerCase()))
    }

    if (!searchType) {
      return items
    }
  }

  useEffect(() => {
    if (searchByTitle && searchByCategory) setFilteredItems(filterBy('BY_TITLE_AND_CATEGORY', items, searchByTitle, searchByCategory))
    if (searchByTitle && !searchByCategory) setFilteredItems(filterBy('BY_TITLE', items, searchByTitle, searchByCategory))
    if (!searchByTitle && searchByCategory) setFilteredItems(filterBy('BY_CATEGORY', items, searchByTitle, searchByCategory))
    if (!searchByTitle && !searchByCategory) setFilteredItems(filterBy(null, items, searchByTitle, searchByCategory))
  }, [items, searchByTitle, searchByCategory])

  return (
    <ShoppingCartContext.Provider value={{
      ....
      filteredItems,
      searchByCategory,
      setSearchByCategory
    }}>
      {children}
    </ShoppingCartContext.Provider>
  )
}
```

## Corrigiendo algunos bugs

1. En Home

```jsx
....

function Home() {
....
  const renderView = () => {
    if (context.filteredItems?.length > 0) {
      return (
        context.filteredItems?.map(item => (
          <Card key={item.id} data={item} />
        ))
      )
    } else {
      return (
        <div>We don't have anything :(</div>
      )
    }
  }
  ....
}

export default Home
```

2. CheckoutSideMenu/index.jsx

```jsx
....

const CheckoutSideMenu = () => {
  const context = useContext(ShoppingCartContext)

  ....

  const handleCheckout = () => {
    const orderToAdd = {
      date: '01.02.23',
      products: context.cartProducts,
      totalProducts: context.cartProducts.length,
      totalPrice: totalPrice(context.cartProducts)
    }

    context.setOrder([...context.order, orderToAdd])
    context.setCartProducts([])
    context.setSearchByTitle(null)
  }

  return (
    ....
  )
}

export default CheckoutSideMenu
```

## Deploy de React en Netlify

1. [Documentacion](https://vitejs.dev/guide/static-deploy.html)
2. [Netlify Get Started](https://docs.netlify.com/cli/get-started/)

# Modulo 5: React con Typescript

Es una buena practica al trabajar con TypeScript, tener un archivo de configuracion para el proyecto. Para aprovechar al maximo el tipado te recomiendo que actives las siguientes opciones en el archivo tsconfig.json

```json
{
  "compilerOptions": {
    ....
    "strict": true,
    "noImplicitAny": true,
    "noImplicitReturns": true,
    ....
  },
  "include": ["src"]
}
```

## Creando una app con React y TypeScript

Para este modulo vamos a utilizar next.js, que es un framework de React que nos permite crear aplicaciones con React y TypeScript de una manera muy sencilla.

[Documentacion](https://nextjs.org/docs/getting-started/installation)

Para crear una aplicacion con next.js, vamos a utilizar el siguiente comando:

```bash
npx create-next-app@latest --ts --use-npm
```

Puedes correr el servidor de desarrollo con el siguiente comando:

```bash
npm run dev
```

Paso a paso de esta clase

1. En tsconfig.json

```json
{
  "compilerOptions": {
    ....
    "strict": true,
    "noImplicitAny": true,
    "noImplicitReturns": true,
    ....
  },
  "include": ["src"]
}
```

2. En el archivo .eslintrc.json. SOLO PARA AMBIENTES DE DESARROLLO

```json
{
  "extends": "next/core-web-vitals",
  "rules": {
    "@next/next/no-img-element": "off",
    "jsx-a11y/alt-text": "off"
  }
}
```

3. Limpiar proyecto

   1. Limpair el archivo pages/index.tsx

   ```jsx
   import Head from "next/head";
   import type { NextPage } from "next";

   const Home: NextPage = () => {
     return (
       <div>
         <Head>
           <title>Create Next App</title>
           <meta name="description" content="Generated by create next app" />
           <link rel="icon" href="/favicon.ico" />
         </Head>

         <main>
           <h1> Hello World </h1>
         </main>

         <footer></footer>
       </div>
     );
   };

   export default Home;
   ```

   2. Eliminar carpeta api
   3. En los styles solo dejar el archivo globals.css completamente vacio

4. Instala tailwind con Next. Apoyate en la documentacion.

## Diferentes formas de definir un componente.

**Formas de definir un componente con TypeScript**

```tsx
import type { FunctionComponent, FC } from "react";

// export const RandomFox = () => {
//   return (
//     <img />
//   )
// }

// Generar un numero aleatorio entre 1 y 122

const random = () => Math.floor(Math.random() * 122) + 1;

export const RandomFox: JSX.Element = () => {
  const image: string = `ruta de la imagen/${random()}.jpg}`;
  return <img src={image} />;
};

// export const RandomFox: FunctionComponent = () => {
//   return (
//     <img />
//   )
// }

// export const RandomFox: FC = () => {
//   return (
//     <img />
//   )
// }
```

## Props en TypeScript

```tsx
export const RandomFox: JSX.Element = (props: { image: string }) => {
  return <img src={props.image} />;
};

// Otra forma
type Props = {
  image: string;
};

export const RandomFox: JSX.Element = (props: Props) => {
  return <img src={props.image} />;
};

// Otra forma
type Props = {
  image: string;
};

export const RandomFox = ({ image }: Props): JSX.Element => {
  return <img src={props.image} />;
};
```

## State con tipos primitivos

Podemos tipar el estado de un componente de la siguiente manera:

```tsx
const [state, setState] = useState<string[]>([]);
```

```tsx
import { useState } from "react";

type State = {
  count: number;
};

export const Counter = () => {
  const [state, setState] = useState<State>({
    count: 0,
  });

  const handleClick = () => {
    setState({
      count: state.count + 1,
    });
  };

  return (
    <div>
      <h1>Counter: {state.count}</h1>
      <button onClick={handleClick}>Increment</button>
    </div>
  );
};
```

o bien, si quieres guardar un arreglo de objetos, puedes hacerlo de la siguiente manera:

```tsx
import { useState } from "react";

type State = {
  products: Array<{
    id: number;
    title: string;
    price: number;
  }>;
};

// Otra forma
// type state = {
//     id: number,
//     title: string,
//     price: number
// }

// useState<Array<state>>

export const Counter = () => {
  const [state, setState] = useState<State>({
    products: [
      {
        id: 1,
        title: "Producto 1",
        price: 100,
      },
      {
        id: 2,
        title: "Producto 2",
        price: 200,
      },
    ],
  });

  const handleClick = () => {
    setState({
      products: [
        ...state.products,
        {
          id: 3,
          title: "Producto 3",
          price: 300,
        },
      ],
    });
  };

  return (
    <div>
      <h1>Counter: {state.count}</h1>
      <button onClick={handleClick}>Increment</button>
    </div>
  );
};
```

## Tipos para eventos y callback de escuchadores

A medida que desarrollamos aplicaciones en TypeScript, una de las tareas más importantes es asegurarnos de que estamos trabajando con tipos de datos precisos y seguros. Esto es particularmente importante cuando trabajamos con eventos y callbacks de escuchadores en React, ya que necesitamos especificar el tipo de evento que se está produciendo.

Afortunadamente, muchas librerías y frameworks modernos ya proporcionan tipos de datos precisos y completos para eventos. Esto significa que podemos confiar en que las funciones que estamos utilizando son seguras y precisas.

Para asegurarnos de que estamos utilizando los tipos de datos correctos para eventos, necesitamos asegurarnos de que nuestra configuración de TypeScript incluya las librerías que estamos utilizando. Podemos hacer esto especificando las librerías que estamos usando en nuestro archivo tsconfig.json.

```json
{
  "compilerOptions": {
    ...
    "lib": ["DOM", "DOM.Iterable", "ESNext"]**, // especificamos las librerías que usamos
    ...
  },
  ...
}
```

Una vez que hemos configurado nuestro proyecto correctamente, podemos inspeccionar los tipos de eventos utilizando el editor de código que estemos utilizando. Por ejemplo, si queremos saber el tipo de datos que se produce en un evento onClick de un botón, podemos simplemente hacer hover sobre el método onClick y buscar su definición.

El editor de código nos mostrará la definición del método onClick, junto con información sobre su tipo de datos:

En este caso, el tipo de datos del evento es `React.MouseEvent<HTMLButtonElement>`. Esto significa que podemos utilizar este tipo de datos para especificar el tipo que se produce en nuestro callback de escuchador de eventos.

Por ejemplo, podemos definir una función addNewFox que se llama cuando se hace clic en un botón. Para especificar el tipo de datos del evento que se produce, podemos incluir React.`MouseEvent<HTMLButtonElement>` como argumento de nuestra función:

```ts
function App(): JSX.Element {
  const addNewFox = React.MouseEvent<HTMLButtonElement>: void => {
    event.preventDefault()
    const target = event.target

    // ...
  }

  return (
    // JSX del componente App...
  )
}
```

En este ejemplo, la función addNewFox toma un argumento de tipo `React.MouseEvent<HTMLButtonElement>`. Esto nos permite acceder a las propiedades del evento de manera segura y precisa, sin tener que utilizar tipos de datos genéricos como any.

También, podemos hacer la importación de los tipos de manera directa:

```ts
// importación del tipo desde React
import type { MouseEvent } from "react"

function App(): JSX.Element {
  // Evitamos escribir de donde viene "React"
	const addNewFox = (event: MouseEvent<HTMLButtonElement>): void => {
    event.preventDefault()
    const target = event.target

    // ...
  }

  return (
    // JSX del componente App...
  )
}
```

# Modulo 6: React Native

## Instalacion del CLI de React Native Expo

[Documentacion](https://reactnative.dev/docs/environment-setup?guide=quickstart)

## Instalacion de Android Studio para utilizar los emuladores

[Documentacion](https://developer.android.com/studio?hl=es-419)

Despues de intalar android studio en la pantalla inicial

1. Configuraciones
2. AVD Manager
3. Create Virtual Device
4. Phone
5. Nexus 6
6. Seleccionar sistema operativo android
7. Descargar
8. Terminar y luego darle click en el boton de play (Ya puedes cerrar android studio y dejar abierto solo la pantalla del emulador)

Puedes cargar la aplicacion en el emulador con el siguiente comando:

```bash
npm run android
```

## Pruebas en un dispositivo fisico

1. Descargar aplicacion Expo Go en el celular
2. Correr el siguiente comando

```bash
npm start
```

3. Escanear el codigo QR que aparece en la terminal
4. Listo

## Estructura de un proyecto

1. El archivo app.json es el archivo de configuracion de la aplicacion. En el puedes configurar el nombre de la aplicacion, el icono, el color de fondo, la orientacion y otras cosas
2. App.js es el archivo principal de la aplicacion. En el se encuentra el componente principal de la aplicacion
3. React Navie utiliza una estructura un poco diferente a React. Por ejemplo, en reacty html puede colocar un parrafo con la etiqueta `<p>` pero en react native no existe esa etiqueta. En su lugar, se utiliza el componente `<Text>` para mostrar texto en pantalla.
4. La funcion StyleSheet.create() nos permite crear estilos para nuestros componentes. Esta funcion recibe un objeto con los estilos que queremos aplicar a nuestro componente. Por ejemplo:

```jsx
const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: "#fff",
    alignItems: "center",
    justifyContent: "center",
  },
});
```

## Creacion de componentes

Debes crear una carpeta llamada src y dentro de ella crear una carpeta llamada components. Dentro de esta carpeta puedes crear todos los componentes que quieras. La estructura de un componente es la siguiente:

```jsx
import React from "react";
import { TextInput, Button, Text } from "react-native";

const Component = () => {
  return (
    <View>
      <Text>Component</Text>
      <TextInput placeholder="email" />
      <TextInput placeholder="contrasena" />
      <Button title="Enviar" onPress={()=>console.log('Enviado')}>
    </View>
  );
};

export default Component;
```

Puedes importar componentes de la siguiente manera:

```jsx
import React from "react";
import { TextInput, Button, Text } from "react-native";
import Component from "./components/Component";

const App = () => {
  return (
    <>
      <Component />
    </>
  );
};

export default App;
```

## Propiedades entre componentes

```jsx
import React from "react";
import { Text } from "react-native";

export default function Saludar(props) {
  const { name } = props;

  return <Text>Hola {name}</Text>;
}
```

```jsx
import React from "react";
import { StyleSheet, Text, View } from "react-native";
import Saludar from "./src/components/Saludar";

export default function App() {
  return (
    <View style={styles.container}>
      <Text>Curso React Native</Text>
      <Saludar name="Agustin Navarro Galdon" />
      <Saludar name="Carlos Navarro" />
      <Saludar name="Andres Navarro" />
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: "#fff",
    alignItems: "center",
    justifyContent: "center",
  },
});
```

## Propiedades por defecto

```jsx
import { Text } from "react-native";

const Saludar = ({ name = "default name" }) => {
  return <Text> Hola {name}</Text>;
};

export default Saludar;
```

## Instalando y configurando React Navigation

[Documentacion](https://reactnavigation.org/docs/getting-started)

**Instalar Stacks**

1. [Documentacion](https://reactnavigation.org/docs/hello-react-navigation)
2. [Drawer Navigation](https://reactnavigation.org/docs/drawer-based-navigation)
3. [Tab Navigation](https://reactnavigation.org/docs/tab-based-navigation)

Debemos encerrar nuestra aplicacion en el componente NavigationContainer

```jsx
import * as React from "react";
import { NavigationContainer } from "@react-navigation/native";

export default function App() {
  return (
    <NavigationContainer>{/* Rest of your app code */}</NavigationContainer>
  );
}
```

## Stack de navegacion

En src, crea la carpeta screens y dentro de ella crea el archivo HomeScreen.jsx

```jsx
import React from "react";
import { StyleSheet, Text, View, Button } from "react-native";

const HomeScreen = (props) => {
  const { navigation } = props;

  const goToPage = () => {
    navigation.navigate("Settings");
  };

  return (
    <View>
      <Text>Home Screen</Text>
      <Button title="Ir a Settings" onPress={goToPage} />
    </View>
  );
};

export default HomeScreen;
```

Crear SettingsScreen.jsx

```jsx
import React from "react";
import { StyleSheet, Text, View } from "react-native";

const SettingsScreen = () => {
  return (
    <View>
      <Text>Settings Screen</Text>
    </View>
  );
};

export default SettingsScreen;
```

En src crear carpeta navigation y dentro de ella crear el archivo StackNavigation.jsx

```jsx
import React from "react";
import { createStackNavigator } from "@react-navigation/stack";
import HomeScreen from "../screens/HomeScreen";
import SettingsScreen from "../screens/SettingsScreen";

const Stack = createStackNavigator();

const StackNavigation = () => {
  return (
    <Stack.Navigator initialRouteName="Home">
      <Stack.Screen name="Home" component={HomeScreen} />
      <Stack.Screen name="Settings" component={SettingsScreen} />
    </Stack.Navigator>
  );
};

export default StackNavigation;
```

En App.js

```jsx
import React from "react";
import { StyleSheet, Text, View } from "react-native";
import { NavigationContainer } from "@react-navigation/native";
import StackNavigation from "./src/navigation/StackNavigation";

export default function App() {
  return (
    <NavigationContainer>
      <StackNavigation />
    </NavigationContainer>
  );
}
```

## Tab Navigation y SafeAreaView

En navigation crear el archivo TabNavigation.js

```js
import React from "react";
import { createBottomTabNavigator } from "@react-navigation/bottom-tabs";
import HomeScreen from "../screens/HomeScreen";
import SettingsScreen from "../screens/SettingsScreen";

const Tab = createBottomTabNavigator();

const TabNavigation = () => {
  return (
    <Tab.Navigator>
      <Tab.Screen name="Home" component={HomeScreen} />
      <Tab.Screen name="Settings" component={SettingsScreen} />
    </Tab.Navigator>
  );
};

export default TabNavigation;
```

En HomeScreen.jsx

```jsx
....
import { View, Text, Button, SafeAreaView } from "react-native";

const HomeScreen = (props) => {
  const { navigation } = props;

  const goToPage = () => {
    navigation.navigate("Settings");
  };

  return (
    <SafeAreaView>
        <Text>Home Screen</Text>
        <Button title="Ir a Settings" onPress={goToPage} />
    </SafeAreaView>
  );
};

export default HomeScreen;
```

En App.js

```jsx
....
import TabNavigation from "./src/navigation/TabNavigation";

export default function App() {
  return (
    <NavigationContainer>
      <TabNavigation />
    </NavigationContainer>
  );
}
```

## Drawer Navigation

En navigation crear el archivo DrawerNavigation.js

```js
import React from "react";
import { createDrawerNavigator } from "@react-navigation/drawer";
import HomeScreen from "../screens/HomeScreen";
import SettingsScreen from "../screens/SettingsScreen";

const Drawer = createDrawerNavigator();

const DrawerNavigation = () => {
  return (
    <Drawer.Navigator>
      <Drawer.Screen name="Home" component={HomeScreen} />
      <Drawer.Screen name="Settings" component={SettingsScreen} />
    </Drawer.Navigator>
  );
};

export default DrawerNavigation;
```

En App.js

```jsx
....
import DrawerNavigation from "./src/navigation/DrawerNavigation";

export default function App() {
  return (
    <NavigationContainer>
      <DrawerNavigation />
    </NavigationContainer>
  );
}
```

## Practica: Configuracion de React Navigation

1. Instalar y configurar React Navigation
2. En este caso, vamos a utilizar un boton tab con iconos, por lo tanto debemos instalar la libreria de iconos

```bash
npm install react-native-vector-icons/Ionicons
```

[Documentacion](https://platzi.com/new-home/clases/2557-react-native-listas-apis/42913-configuracion-de-react-navigation/)

3. en src/navigation crear el archivo TabNavigation.js

```js
import React from "react";
import { createBottomTabNavigator } from "@react-navigation/bottom-tabs";
import FavoritesScreen from "../screens/FavoritesScreen";
import PokedexScreen from "../screens/PokedexScreen";
import AccountScreen from "../screens/AccountScreen";

import { Ionicons } from "@expo/vector-icons";

const Tab = createBottomTabNavigator();

const TabNavigation = () => {
  return (
    <Tab.Navigator>
      <Tab.Screen name="Favorites" component={Favorites} />
      <Tab.Screen name="Pokedex" component={Pokedex} />
      <Tab.Screen name="Account" component={Account} />
    </Tab.Navigator>
  );
};

export default TabNavigation;
```

En screens, crear archivo AccountScreen, PokedexScreen, FavoritesScreen con la estructura basica de un componente

```jsx
import React from "react";
import { SafeAreaView, Text } from "react-native";

const AccountScreen = () => {
  return (
    <SafeAreaView>
      <Text>AccountScreen</Text>
    </SafeAreaView>
  );
};

export default AccountScreen;
```

[Posible error](https://platzi.com/comentario/3056174/)
