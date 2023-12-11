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
  - [Instalacion de React con Vite y TailwindCSS](#instalacion-de-react-con-vite-y-tailwindcss)
    - [Que es Vite](#que-es-vite)
    - [Que es TailwindCSS](#que-es-tailwindcss)
    - [Crear un proyecto con Vite](#crear-un-proyecto-con-vite)
    - [Instalacion de TailwindCSS](#instalacion-de-tailwindcss)
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
import './CreateToDoButton.css'

function CreateToDoButton() {
  return <button className="CreateToDoButton" onClick={() => {
    console.log('Le diste click');
  }}>+</button>;
}

export { CreateToDoButton };
```

2. **onChange**: se ejecuta cuando el valor de un elemento cambia, como un campo de texto.

```jsx
import "./ToDoSearch.css";

function ToDoSearch() {
  return <input placeholder="Cortar cebolla" className="TodoSearch" onChange={(event) => {
    console.log(event.target.value);
  }} />;
}

export { ToDoSearch };
```

*Nota: event.target hace referencia al elemento que disparo el evento. event.target.value se usa para obtener el valor actual del elemento de entrada.*

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
]

function App() {
  const [toDos, setToDos] = React.useState(defaultToDos);
  const [searchValue, setSearchValue] = React.useState('');

  const completedToDos = toDos.filter((toDo) => toDo.completed).length;
  const totalToDos = toDos.length;
  
  console.log('Los usuarios buscan todos de ' + searchValue);

  return (
    <>
      <ToDoCounter completed={completedToDos} total={totalToDos} />
      <ToDoSearch 
        searchValue={searchValue}
        setSearchValue={setSearchValue}
      />
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
import './ToDoItem.css'

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

*Nota: si quieres iconos dinamicos, por ejemplo, que cambien de color, debes quitar en cada archivo svg
debes eliminar la propiedad fill y posteriormente, incluirla con ReactJS como lo vamos hacer*

1. Crear TodoIcon.js. Este componente recibe como prop el tipo de icono que se va a renderizar y el color del icono.

```jsx
// src/TodoIcon.js
import { ReactComponent as CheckSVG } from './check.svg';
import { ReactComponent as DeleteSVG } from './delete.svg';
import './TodoIcon.css';

const iconTypes = {
  "check": <CheckSVG />,
  "delete": <DeleteSVG />,
};

function TodoIcon({ type }) {
  return (
    <span className={`Icon-container Icon-container-${type}`}>
      {iconTypes[type]}
    </span>
  )
}

export { TodoIcon };
```

```jsx
import React from 'react';
import { TodoIcon } from './TodoIcon';

function CompleteIcon() {
  return (
    <TodoIcon
      type="check"
    />
  );
}

export { CompleteIcon };
```

```jsx
import React from 'react';
import { TodoIcon } from './TodoIcon';

function DeleteIcon() {
  return (
    <TodoIcon
      type="delete"
    />
  );
}

export { DeleteIcon };
```

#### Iconos con colores dinamicos
1. Crear la propiedad color en ToDoIcon.js y incluir la clase Icon-svg a cada svg, ademas de modificarlos para recibir el parametro color y finalmnente incluir la propiedad fill.

```jsx
// src/TodoIcon.js
import { ReactComponent as CheckSVG } from './check.svg';
import { ReactComponent as DeleteSVG } from './delete.svg';
import './TodoIcon.css';

const iconTypes = {
  "check": (color) => <CheckSVG className="Icon-svg" fill={color}/>,
  "delete": (color) => <DeleteSVG className="Icon-svg" fill={color}/>,
};

function TodoIcon({ type, color, onClick}) {
  return (
    <span className={`Icon-container Icon-container-${type}`} onClick={onClick}>
      {iconTypes[type](color)}
    </span>
  )
}

export { TodoIcon };
```

```jsx
import React from 'react';
import { TodoIcon } from './TodoIcon';

function CompleteIcon({ completed, onComplete }) {
  return (
    <TodoIcon
      type="check"
      color={completed ? 'green' : 'gray'}
      onClick={onComplete}
    />
  );
}

export { CompleteIcon };
```

```jsx
import React from 'react';
import { TodoIcon } from './TodoIcon';

function DeleteIcon({ onDelete }) {
  return (
    <TodoIcon
      type="delete"
      color="gray"
      onClick={onDelete}
    />
  );
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
```

Para obtener un dato del localStorage, podemos utilizar el método getItem:

```jsx
localStorage.getItem('nombre');
```

Para eliminar un dato del localStorage, podemos utilizar el método removeItem:

```jsx
localStorage.removeItem('nombre');
```

En nuestro proyecto, vamos a utilizar el localStorage para guardar los ToDos, de forma que cuando el usuario recargue la página, los ToDos se sigan mostrando.

1. En la consola del navegador vas a crear el array de objetos que contiene los ToDos, y lo vas a guardar en el localStorage utilizando el método setItem:

```jsx
const defaultTodos = [
  { text: 'Cortar cebolla', completed: true },
  { text: 'Tomar el curso de intro a React', completed: false },
  { text: 'Llorar con la llorona', completed: false },
  { text: 'LALALA', completed: false },
];

localStorage.setItem('TODOS_V1', JSON.stringify(defaultTodos));
```

*NOTA: Todo lo que se guarda en localStorage debe ser un string*

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

*Nota: Por convencion las funciones de custom Hooks comienzan con la palabra use*

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

*Nota: Para poder separar la funcion useLocalStorage debes incluir al final del arhivo la exportacion*

```jsx
...
export { useLocalStorage };
```

*Nota: Para poder importar la funcion useLocalStorage debes incluir al final del arhivo la importacion*

```jsx
...
import { useLocalStorage } from './useLocalStorage';
```

Tambien puedes mover la UI de tu componente a un archivo separado, por ejemplo.

1. Crear un archivo AppUI.js

```js
// Todos los imports de React y componentes

function AppUI(
{ totalTodos,
  completedTodos,
  searchValue,
  setSearchValue,
  searchedTodos,
  completeTodo,
  deleteTodo}
) {
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
Los efectos son una característica de React que nos permite ejecutar código cuando se monta, desmonta o actualiza un componente.  Los efectos se utilizan para ejecutar código que necesita acceder al DOM, como por ejemplo, para obtener el tamaño de la ventana, o para ejecutar código asíncrono, como por ejemplo, para obtener datos de una API.

**useEffect**: se ejecuta cuando se monta, desmonta o actualiza un componente.Recibe dos parámetros: una función que se ejecuta cuando se monta, desmonta o actualiza el componente, y una lista de dependencias que se utiliza para indicarle a React cuando debe volver a ejecutar la función. Si la lista de dependencias está vacía, la función se ejecuta solo cuando se monta y desmonta el componente.


```jsx
import React from 'react';

function App() {
  console.log('Log1');
 
  React.useEffect(() => {
    console.log('Log2');
  });  // Si no se pasa un arreglo de dependencias, se ejecuta cuando se monta y desmonta el componente

  React.useEffect(() => {
    console.log('Log2');
  }, []);  // Si se pasa un arreglo de dependencias vacío, se ejecuta solo cuando se monta el componente

  React.useEffect(() => {
    console.log('Log2');
  }, [totalTodos]);  // Si se pasa un arreglo de dependencias con una variable, se ejecuta cuando se monta el componente y cuando cambia el valor de la variable

  console.log('Log3');
  
  return (
    <div>
    </div>
  );
}

export default App;
```

useEffect se utiliza comunmente para obtener datos de una API, por ejemplo:

```jsx
import React from 'react';

function TodoMessage() {
  const [state, setState] = React.useState({});

  React.useEffect(() => {
    fetch('url')
      .then((response) => response.json())
      .then((data) => setState(data));
  }, []);

  return (
    <p>
      {state.message} || "Cargando..."
    </p>
  );
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
import React from 'react';

function EmptyTodos() {
  return (
    <p>¡Crea tu primer TODO!</p>
  );
}

export { EmptyTodos };
```

Crear componente TodosError

```jsx
import React from 'react';

function TodosError() {
  return (
    <p>Error...</p>
  );
}

export { TodosError };
```

Crear componente TodosLoading

```jsx
import React from 'react';
import './TodosLoading.css';

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
  background: linear-gradient(90deg, rgba(250,250,250,1), rgb(200, 199, 199));
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
import React from 'react';
import { useLocalStorage } from './useLocalStorage';

const TodoContext = React.createContext();

function TodoProvider({ children }) {
  const {
    item: todos,
    saveItem: saveTodos,
    loading,
    error,
  } = useLocalStorage('TODOS_V1', []);
  const [searchValue, setSearchValue] = React.useState('');

  const completedTodos = todos.filter(
    todo => !!todo.completed
  ).length;
  const totalTodos = todos.length;

  const searchedTodos = todos.filter(
    (todo) => {
      const todoText = todo.text.toLowerCase();
      const searchText = searchValue.toLowerCase();
      return todoText.includes(searchText);
    }
  );

  const completeTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text === text
    );
    newTodos[todoIndex].completed = true;
    saveTodos(newTodos);
  };

  const deleteTodo = (text) => {
    const newTodos = [...todos];
    const todoIndex = newTodos.findIndex(
      (todo) => todo.text === text
    );
    newTodos.splice(todoIndex, 1);
    saveTodos(newTodos);
  };
  
  return (
    <TodoContext.Provider value={{
      loading,
      error,
      completedTodos,
      totalTodos,
      searchValue,
      setSearchValue,
      searchedTodos,
      completeTodo,
      deleteTodo,
    }}>
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
import React from 'react';
import { TodoContext } from '../TodoContext';
import './TodoCounter.css';

function TodoCounter() {
  const {
    completedTodos,
    totalTodos,
  } = React.useContext(TodoContext);
  
  return (
    <h1 className="TodoCounter">
      Has completado <span>{completedTodos}</span> de <span>{totalTodos}</span> TODOs
    </h1>
  );
}

export { TodoCounter };
```

En el componente TodoSearch
```jsx
import React from 'react';
import { TodoContext } from '../TodoContext';
import './TodoSearch.css';

function TodoSearch() {
  const {
    searchValue,
    setSearchValue,
  } = React.useContext(TodoContext);
  
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
import React from 'react';
import ReactDOM from 'react-dom';
import './Modal.css';

function Modal({ children }) {
  return ReactDOM.createPortal(
    <div className="ModalBackground">
      {children}
    </div>,
    document.getElementById('modal')
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
  background-color: rgba(32,35,41,.8);
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
import './CreateTodoButton.css';

function CreateTodoButton({ setOpenModal }) {
  return (
    <button
      className="CreateTodoButton"
      onClick={
        () => {
          setOpenModal(state => !state);
        }
      }
    >+</button>
  );
}

export { CreateTodoButton };
```

7. Modificar el archivo createTodoButton.css

```css
.CreateTodoButton {
  background-color: #61DAFA;
  box-shadow: 0px 5px 25px rgba(97, 218, 250, 0.5);
  border: none;
  border-radius: 50%;
  cursor: pointer;
  font-size: 50px;
  position: fixed;
  bottom: 24px;
  right: 24px;
  font-weight: bold;
  color: #FAFAFA;
  display: flex;
  justify-content: center;
  align-items: center;
  height: 64px;
  width: 64px;
  z-index: 1;

  transform: rotate(0);
  transition: .3s ease;
}

.CreateTodoButton:hover {
  transform: rotate(224deg);
}
```

## Maquetando formularios en React
- Crear el componente TodoForm/index.js

```jsx
import React from 'react';
import { TodoContext } from '../TodoContext';
import './TodoForm.css';

function TodoForm() {
  const {
    addTodo,
    setOpenModal,
  } = React.useContext(TodoContext);
  const [newTodoValue, setNewTodoValue] = React.useState('');

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
        >Cancelar</button>
        <button
          type="submit"
          className="TodoForm-button TodoForm-button--add"
        >Añadir</button>
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
  color: #1E1E1F;
  margin-bottom: 26px;
}

textarea {
  background-color: #F9FBFC;
  border: 2px solid #202329;
  border-radius: 2px;
  box-shadow: 0px 5px 50px rgba(32, 35, 41, 0.25);
  color: #1E1E1F;
  font-size: 20px;
  text-align: center;
  padding: 12px;
  height: 96px;
  width: calc(100% - 25px);
}

textarea::placeholder {
  color: #A5A5A5;
  font-family: 'Montserrat';
  font-weight: 400;
}

textarea:focus {
  outline-color: #61DAFA;
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
  font-family: 'Montserrat';
}

.TodoForm-button--add {
  background: #61DAFA;
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

## Instalacion de React con Vite y TailwindCSS

### Que es Vite

Vite es un nuevo compilador de código abierto que sirve para crear aplicaciones web modernas con React, Vue, Svelte, Preact y TypeScript. Vite se centra en el tiempo de compilación y el tiempo de ejecución rápido. No es un marco completo, sino más bien un compilador de desarrollo que aprovecha las importaciones nativas de ES Module para lograr un tiempo de compilación rápido y un servidor de desarrollo instantáneo con recarga rápida.

### Que es TailwindCSS

Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite crear rápidamente diseños personalizados y receptivos para sitios web. Tailwind CSS es un framework CSS de utilidad de bajo nivel que le permite crear rápidamente diseños personalizados y receptivos para sitios web.

### Crear un proyecto con Vite

Para crear un proyecto con Vite, debemos tener instalado Node.js y npm. Luego, abrimos una terminal y ejecutamos el siguiente comando:

```bash
npm create vite@latest
```

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