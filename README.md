# Curso de React.js, Vite.js y TailwindCSS
## Tabla de contenido

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
import React from 'react';

const Saludo = (props) => {
  return <p>Hola, {props.nombre}!</p>;
};

export default Saludo;
```

Luego, en otro componente superior (padre), puedes utilizar el componente "Saludo" y pasarle la prop "nombre":

```jsx
import React from 'react';
import Saludo from './Saludo';

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

*Nota:* Para empezar de cero un proyecto puedes eliminar la carpeta assets, limpiar el archivo App.css y el index.css y el App.jsx, debe quedar asi.

```jsx
import './App.css';

function App() {
  return (
    <div className="bg-red-100">
        <h1>Hola Mundo</h1>
    </div>
  );
}

export default App;
```
 




