# Curso de React.js, Vite.js y TailwindCSS

## Tabla de contenido

- [Curso de React.js, Vite.js y TailwindCSS](#curso-de-reactjs-vitejs-y-tailwindcss)
  - [Tabla de contenido](#tabla-de-contenido)
  - [ReactJS](#reactjs)
    - [Que es ReactJS](#que-es-reactjs)
    - [Que es un componente](#que-es-un-componente)
    - [Que son Props](#que-son-props)
    - [Estilos con React](#estilos-con-react)
    - [Interaccion con ReactJS](#interaccion-con-reactjs)
      - [Eventos en React](#eventos-en-react)
    - [Estado](#estado)
    - [Practica: Estados](#practica-estados)
    - [Libreria de iconos](#libreria-de-iconos)
      - [Iconos con colores dinamicos](#iconos-con-colores-dinamicos)
  - [Custom Hooks](#custom-hooks)
  - [Organizacion de archivos](#organizacion-de-archivos)
  - [Efectos en React](#efectos-en-react)
    - [Implementando estados de carga y error en la aplicacion ToDos](#implementando-estados-de-carga-y-error-en-la-aplicacion-todos)
  - [React Context](#react-context)
  - [React Portals](#react-portals)
  - [Maquetando formularios en React](#maquetando-formularios-en-react)
  - [Deploy de la aplicacion](#deploy-de-la-aplicacion)
  - [Versiones de React](#versiones-de-react)
  - [Creando proyectos de React](#creando-proyectos-de-react)
  - [TailwindCSS](#tailwindcss)
    - [Mobile first](#mobile-first)
    - [Utility first (framework basado en utilidades)](#utility-first-framework-basado-en-utilidades)
  - [Instalacion de TailwindCSS](#instalacion-de-tailwindcss)
    - [Directivas de tailwindcss](#directivas-de-tailwindcss)
    - [Paleta de colores](#paleta-de-colores)
    - [Medidas y breakpoints](#medidas-y-breakpoints)
    - [Flexbox](#flexbox)
    - [Plugins oficiales de Tailwind CSS](#plugins-oficiales-de-tailwind-css)
  - [Aplicacion del modulo Platzi Travel](#aplicacion-del-modulo-platzi-travel)
    - [Design System](#design-system)
  - [Seccion Home Mobile](#seccion-home-mobile)
    - [width](#width)
    - [height](#height)
    - [flex direction](#flex-direction)
    - [Alinear elementos verticalmente](#alinear-elementos-verticalmente)
    - [Margen interno: padding](#margen-interno-padding)
    - [Espacio entre elementos en flex](#espacio-entre-elementos-en-flex)
    - [Borde de un elemento](#borde-de-un-elemento)
    - [Borde redondeado](#borde-redondeado)
    - [Sombra de caja de un elemento](#sombra-de-caja-de-un-elemento)
    - [Color de fondo](#color-de-fondo)
    - [Grosor de la fuente](#grosor-de-la-fuente)
    - [Color de texto](#color-de-texto)
    - [Tamaño de fondo](#tamaño-de-fondo)
  - [Componentes card mobile](#componentes-card-mobile)
  - [Extraccion de componentes a clases](#extraccion-de-componentes-a-clases)
  - [Seccion recomendados mobile](#seccion-recomendados-mobile)
  - [Animaciones con tailwind](#animaciones-con-tailwind)
    - [Focus](#focus)
    - [Focus within](#focus-within)
    - [Ring](#ring)
  - [Seccion rentas destacadas](#seccion-rentas-destacadas)
  - [Seccion preguntas frecuentes](#seccion-preguntas-frecuentes)
  - [Seccion footer](#seccion-footer)
  - [TabBar](#tabbar)
  - [Responsive Design](#responsive-design)
  - [Creando la navbar](#creando-la-navbar)
  - [Agregando el dark mode](#agregando-el-dark-mode)
  - [Preparando para produccion](#preparando-para-produccion)
  - [Migrar desde tailwindcss 2.x a 3.x](#migrar-desde-tailwindcss-2x-a-3x)
  - [Instalacion de React con Vite y TailwindCSS ### Que es Vite Vite es un](#instalacion-de-react-con-vite-y-tailwindcss--que-es-vite-vite-es-un)
    - [Instalacion de TailwindCSS](#instalacion-de-tailwindcss-1)
  - [Enlaces de interes](#enlaces-de-interes)

## ReactJS

### Que es ReactJS

React es una biblioteca de JavaScript de código abierto diseñada para crear interfaces de usuario con el objetivo de facilitar el desarrollo de aplicaciones en una sola página. Es mantenido por Facebook y la comunidad de software libre, han participado en el proyecto más de mil desarrolladores diferentes.

### Que es un componente

Un componente es una pieza de código reutilizable que se puede utilizar para construir elementos de interfaz de usuario. Los componentes son como funciones de JavaScript. Aceptan entradas arbitrarias (llamadas "props") y devuelven elementos React que describen lo que debería aparecer en la pantalla.

[¿Cuándo crear un Componente? Estructura, Organización y Tipos de Componentes en React](https://platzi.com/blog/estructura-organizacion-y-tipos-de-componentes-en-react/)

### Que son Props

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

### Estilos con React

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

1. [**Practica: Estilos componentes ToDo Curso Platzi**](https://github.com/platzi/curso-react-intro/tree/04-css)
2. [Google Fonts](https://fonts.google.com/)

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

### Interaccion con ReactJS

Los eventos son acciones que suceden en el navegador que pueden ser detectadas por React y utilizadas para ejecutar código cuando ocurren. Algunos ejemplos de eventos son: hacer clic en un botón, pasar el mouse sobre un elemento, escribir en un campo de texto, etc.

#### Eventos en React

1. **onClick**: se ejecuta cuando se hace clic en un elemento.

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

2. **onChange**: se ejecuta cuando el valor de un elemento cambia, como un campo de texto.

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

_Nota: event.target hace referencia al elemento que disparo el evento. event.target.value se usa para obtener el valor actual del elemento de entrada._

### Estado

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

### Libreria de iconos

Existen diferentes librerias de iconos que podemos utilizar en nuestros proyectos de React,una de las mas populares es React Icons, que nos permite utilizar iconos de diferentes librerias como Font Awesome, Material Design, Ionicons, etc.:

1. React Icos: [https://react-icons.github.io/react-icons/](https://react-icons.github.io/react-icons/)

Aveces, no se puede utilizar iconos en librerias por que desde el area de diseño nos entregan iconos personalizados. En estos casos, podemos 'crear nuestra propia libreria de iconos' utilizando componentes de React.

Primero debes incluir los svg en la carpeta src.

_Nota: si quieres iconos dinamicos, por ejemplo, que cambien de color, debes quitar en cada archivo svg
debes eliminar la propiedad fill y posteriormente, incluirla con ReactJS como lo vamos hacer_

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

#### Iconos con colores dinamicos

1. Crear la propiedad color en ToDoIcon.js y incluir la clase Icon-svg a cada svg, ademas de modificarlos para recibir el parametro color y finalmnente incluir la propiedad fill.

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

````jsx
import { CompleteIcon } from './CompleteIcon'
import { DeleteIcon } from './DeleteIcon'
import './TodoItem.css';

function TodoItem(props) {
  return (
    <li className="TodoItem">
      <CompleteIcon
        completed={props.completed}
        onComplete={props.onComplete}
      />

      <p className={`TodoItem-p ${props.completed && "TodoItem-p--complete"}`}>
        {props.text}
      </p>

      <DeleteIcon
        onDelete={props.onDelete}
      />
    </li>
  );
}

export { TodoItem };

## LocalStorage
Es una API que nos permite almacenar datos en el navegador de forma persistente. Los datos almacenados en el localStorage no se eliminan al cerrar el navegador, ni al apagar el computador, ni al reiniciar el sistema operativo. Los datos almacenados en el localStorage permanecen ahí hasta que se borren manualmente, o hasta que se borren utilizando código.

Para acceder al localStorage, lo podemos hacer desde la consola del navegador, utilizando el objeto localStorage. Por ejemplo, para guardar un dato en el localStorage, podemos utilizar el método setItem:

```jsx
localStorage.setItem('nombre', 'Juan');
````

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

_NOTA: Todo lo que se guarda en localStorage debe ser un string_

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

Los Custom Hooks son una característica de React que nos permite extraer lógica de componentes en funciones reutilizables. Los Custom Hooks son funciones de JavaScript que utilizan otras características de React, como los Hooks, y que nos permiten crear componentes personalizados.

_Nota: Por convencion las funciones de custom Hooks comienzan con la palabra use_

1. Crear el custom hook useLocalStorage

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

_Nota: Para poder separar la funcion useLocalStorage debes incluir al final del arhivo la exportacion_

```jsx
...
export { useLocalStorage };
```

_Nota: Para poder importar la funcion useLocalStorage debes incluir al final del arhivo la importacion_

```jsx
...
import { useLocalStorage } from './useLocalStorage';
```

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

**useEffect**: se ejecuta cuando se monta, desmonta o actualiza un componente.Recibe dos parámetros: una función que se ejecuta cuando se monta, desmonta o actualiza el componente, y una lista de dependencias que se utiliza para indicarle a React cuando debe volver a ejecutar la función. Si la lista de dependencias está vacía, la función se ejecuta solo cuando se monta y desmonta el componente.

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

### Implementando estados de carga y error en la aplicacion ToDos

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

Los Portales son una característica de React que nos permite renderizar un componente en cualquier parte del DOM, incluso fuera del contenedor principal de la aplicación.

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

## Maquetando formularios en React

- Crear el componente TodoForm/index.js

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

- Crear el componente TodoForm/TodoForm.css

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

- Modificar AppUI.js

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

- Modificar TodoContext.js

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

## Deploy de la aplicacion

1. En el archivo package.json y modifica la propiedad Homepage para desplegar en github

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
   W
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

1. Crear un proyecto con create-react-app

```bash
npx create-react-app nombre_del_proyecto
```

2. Crear un proyecto con next.js

```bash
npm create-next-app@latest nombre_proyecto
```

## TailwindCSS

Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite crear rápidamente diseños personalizados y receptivos para sitios web. Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite crear rápidamente diseños personalizados y receptivos para sitios web.

### Mobile first

Mobile first es una técnica de diseño que consiste en diseñar primero la versión móvil de un sitio web, y luego ir agregando características para las versiones de escritorio y tablet.

### Utility first (framework basado en utilidades)

Un framework basado en utilidades es un framework CSS que se basa en clases de utilidad para crear diseños. Por ejemplo, para crear un layout de dos columnas, podemos utilizar las clases de utilidad de Tailwind CSS:

```html
<div class="flex">
  <div class="w-1/2">...</div>
  <div class="w-1/2">...</div>
</div>
```

[Documentacion](https://tailwindcss.com/docs/utility-first)

## Instalacion de TailwindCSS

1. Crear carpeta PlatziTravel y crear un proyecto con npm

```bash
npm init -y
```

2. Crear carpeta public y dentro de ella crear el archivo index.html
3. Crear carpeta src y dentro de ella crear el archivo styles.css
4. En la carpeta src crear el archivo index.js
5. Instalar tailwindcss

[Documentacion](https://tailwindcss.com/docs/installation)

### Directivas de tailwindcss

[Documentacion](https://tailwindcss.com/docs/functions-and-directives)

### Paleta de colores

[Documentacion](https://tailwindcss.com/docs/customizing-colors)

[Tailwind play](https://play.tailwindcss.com/)

[Coolors](https://coolors.co/)

### Medidas y breakpoints

1. **Breakpoints**
   Un breakpoint es un punto en el que se cambia el diseño de una página web. Por ejemplo, en una página web con un diseño de dos columnas, en la versión móvil, las dos columnas se muestran una debajo de la otra, mientras que en la versión de escritorio, las dos columnas se muestran una al lado de la otra.

Podemos utilizar los breakpoints de Tailwind CSS para crear diseños responsivos.

[Breakpoints mas comunes](https://tailwindcss.com/docs/responsive-design)

2. **Medidas**
   [Documentacion](https://tailwindcss.com/docs/width)

### Flexbox

[Documentacion](https://tailwindcss.com/docs/flex-direction)

_Nota: para separar los elementos en el tipo de display flex puedes utilizar space-x-{medida}_

1. justify-content: se utiliza para alinear los elementos horizontalmente

2. align-items: se utiliza para alinear los elementos verticalmente

### Plugins oficiales de Tailwind CSS

[Documentacion](https://tailwindcss.com/docs/plugins)

## Aplicacion del modulo Platzi Travel

[Figma](https://www.figma.com/file/aPbr2Rhd5SCUjNYu6NRPPB/Platzi-Travel-Mockups?node-id=0%3A1&mode=dev)

Debes descargar las imagenes y los svg que vamos a utilizar en el proyecto desde el repositorio de github. Los archivos .png y .jpg van en la carpeta public/img y los archivos public/svg van en la carpeta icons.

### Design System

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

## Seccion Home Mobile

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

**Documentacion**

### [width](https://tailwindcss.com/docs/width)

### [height](https://tailwindcss.com/docs/height)

### [flex direction](https://tailwindcss.com/docs/flex-direction)

### [Alinear elementos verticalmente](https://tailwindcss.com/docs/align-items)

### [Margen interno: padding](https://tailwindcss.com/docs/padding)

### [Espacio entre elementos en flex](https://tailwindcss.com/docs/space)

### [Borde de un elemento](https://tailwindcss.com/docs/outline-style)

### [Borde redondeado](https://tailwindcss.com/docs/border-radius)

### [Sombra de caja de un elemento](https://tailwindcss.com/docs/box-shadow)

### [Color de fondo](https://tailwindcss.com/docs/background-color)

### [Grosor de la fuente](https://tailwindcss.com/docs/font-weight)

### [Color de texto](https://tailwindcss.com/docs/text-color)

### [Tamaño de fondo](https://tailwindcss.com/docs/background-size)

## Componentes card mobile

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

## Seccion recomendados mobile

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

**Documentacion**

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

**Documentacion**

1. [Primera animacion con tailwind](https://tailwindcss.com/docs/transition-property)
2. [Trasladar un elemento con transformacion](https://tailwindcss.com/docs/translate)
3. [aumentar tamaño del elementos animacion](https://tailwindcss.com/docs/scale)

_transform: Habilita la transformación CSS en el elemento. Esto es necesario para aplicar las clases relacionadas con transformaciones, como hover:-translate-y-1 y hover:scale-110_

_transition-all: Aplica la transición a todas las propiedades CSS, lo que significa que cualquier cambio en el estilo del botón será animado con la transición definida anteriormente._

### Focus

En Tailwind CSS, la clase focus se utiliza para aplicar estilos específicamente cuando un elemento tiene el enfoque. Este enfoque puede ocurrir, por ejemplo, cuando un usuario interactúa con un elemento utilizando el teclado (por ejemplo, al navegar por la página utilizando la tecla "Tab").

Cuando aplicas la clase focus en Tailwind CSS, estás indicando que los estilos asociados a esa clase deben aplicarse cuando el elemento está enfocado.

Por ejemplo, puedes tener una clase como focus:outline-none, que quitará el contorno predeterminado que aparece al enfocar un elemento. Esto puede ser útil para mejorar la accesibilidad y proporcionar una experiencia de usuario más limpia.

### Focus within

En Tailwind CSS, la clase `focus-within` se utiliza para aplicar estilos a un elemento cuando cualquier elemento descendiente de ese elemento tiene el enfoque. Esto es útil cuando deseas estilizar un contenedor basándote en el estado de los elementos hijos que están enfocados.

Por ejemplo, si tienes un contenedor que contiene varios elementos y deseas aplicar estilos al contenedor cuando alguno de sus elementos hijos tiene el enfoque, puedes usar la clase `focus-within`.

Ejemplo:

```html
<div class="focus-within:bg-gray-200">
  <label for="username">Nombre de usuario:</label>
  <input type="text" id="username" class="focus:outline-none" />
</div>
```

En este ejemplo, el fondo del contenedor cambiará a gris (`bg-gray-200`) cuando el input con `id="username"` está enfocado. La clase `focus-within` se aplica al contenedor y se combina con la clase de color de fondo específica (`bg-gray-200`). También se utiliza la clase `focus:outline-none` en el input para quitar el contorno predeterminado cuando está enfocado.

En resumen, `focus-within` es útil para aplicar estilos al contenedor basándote en el estado de enfoque de sus elementos hijos.

### Ring

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

## Seccion rentas destacadas

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

## Seccion preguntas frecuentes

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

## Seccion footer

```html
<footer class="w-full h-auto bg-gray-50 px-6 space-y-2 mt-6 pt-4">
  <p class="text-lg">Acerca De</p>
  <p class="text-sm text-gray-300">Inversionistas</p>
  <p class="text-sm text-gray-300">Empleos</p>
  <p class="text-sm text-gray-300">Términos y condiciones</p>
  <p class="text-sm text-gray-300">Platzi Travel, Inc.</p>
</footer>
```

## TabBar

```html
<div class="w-full h-16 bg-white fixed left-0 bottom-0 shadow-md flex items-center justify-around" id="tab_bar">
   <a href="#home">
    <svg width="30" height="30" viewBox="0 0 20 20" fill="none" xmlns="">
  ....
</div>
```

## Responsive Design

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

## Creando la navbar
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

## Agregando el dark mode
[Documentacion](https://tailwindcss.com/docs/dark-mode)

## Preparando para produccion
[Documentacion](https://tailwindcss.com/docs/optimizing-for-production)

## Migrar desde tailwindcss 2.x a 3.x
[Documentacion](https://tailwindcss.com/docs/upgrade-guide#configure-content-sources)


## Instalacion de React con Vite y TailwindCSS ### Que es Vite Vite es un

nuevo compilador de código abierto que sirve para crear aplicaciones web
modernas con React, Vue, Svelte, Preact y TypeScript. Vite se centra en el
tiempo de compilación y el tiempo de ejecución rápido. No es un marco
completo, sino más bien un compilador de desarrollo que aprovecha las
importaciones nativas de ES Module para lograr un tiempo de compilación rápido
y un servidor de desarrollo instantáneo con recarga rápida. ### Que es
TailwindCSS Tailwind CSS es un framework CSS de utilidad de bajo nivel que le
permite crear rápidamente diseños personalizados y receptivos para sitios web.
Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite
crear rápidamente diseños personalizados y receptivos para sitios web. ###
Crear un proyecto con Vite Para crear un proyecto con Vite, debemos tener
instalado Node.js y npm. Luego, abrimos una terminal y ejecutamos el siguiente
comando: ```bash npm create vite@latest

</div>
````

### Instalacion de TailwindCSS

[https://tailwindcss.com/docs/guides/vite](Documentacion oficial)

_Nota:_ Para empezar de cero un proyecto puedes eliminar la carpeta assets, limpiar el archivo App.css y el index.css y el App.jsx, debe quedar asi.

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

## Enlaces de interes

1. [Google Fonts](https://fonts.google.com/)
2. [Repositorio Aplicacion ToDos](https://github.com/platzi/curso-react-intro)
3. [Figma Aplicacion ToDos](https://www.figma.com/file/3aZkIjXMEzBDACmWxqUVes/TODO-Machine-Mockup?node-id=0%3A1&mode=dev)
4. [Figma 2 Aplicacion ToDos](https://www.figma.com/proto/3aZkIjXMEzBDACmWxqUVes/TODO-Machine-Mockup?type=design&amp%3Bnode-id=1-3&amp%3Bt=NH0HT6nS2TxaLKp4-1&amp%3Bscaling=min-zoom&amp%3Bpage-id=0%3A1&amp%3Bstarting-point-node-id=1%3A3&amp%3Bmode=design&node-id=1-3&starting-point-node-id=1%3A3)
5. [Reppositorio Aplicacion Platzi Travel](https://github.com/platzi/PlatziTravel/tree/main)

5. [Repositorio Tienda en linea con React](https://github.com/platzi/curso-react-practico/tree/master)
