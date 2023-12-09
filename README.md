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

function TodoIcon({ type, color}) {
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

function CompleteIcon({ completed, onComplete }) {
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

function DeleteIcon({ onDelete }) {
  return (
    <TodoIcon
      type="delete"
    />
  );
}

export { DeleteIcon };
```

#### Iconos con colores dinamicos



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
