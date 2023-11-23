# React Interview

### What is React.js ?

It's a popular, component-based, declarative, state-driven, one-way data flow javascript library for building user interfaces.

### Important concept :

1. **Library or framework:**
   It's a famous **JS library**, like a toolbox with different tools you can install. When you put all the tools togather, React acts like a complete framewormk.

2. **Components based:**
   A component is a small re-useable piece of code that can be used again and again. Components are the building blocks of User Interface in React.

3. **Declarative:**
   **"Do not touch the DOM, I will do all the work for you"**, which means we have to understand the rendering approachs. **Vanilla JS (Imperative approach) and React JS (Declarative approach)**, which means developers describe how the user interface should look based on its current state, and React takes care of updating the **DOM (Document Object Model)** accordingly. This Declarative nature of React makes it easier to build and maintain complex UIs.

4. **State driven:**
   The main goal of React is to sync the data with User Interface. In React, you can call the **data as state**, because state is used to store data. So the **DOM manipulation** part is handled by the state in React.

5. **One-way data flow:**
   React enforces a **unidirectional data flow**. Data flows from the top-level component down to child components. Parent components pass data to their children via props, and children communicate back to parents through callbacks.

### What is JSX ?

JSX is a syntax extension for JavaScript that allows developers to write HTML-like code within JavaScript. JSX makes it easy to express the component hierarchy and provides a clear visualization of the UI structure.

### Components :

Components are the building blocks of React applications. They are self-contained pieces of code that can be reused and combined to create complex UIs. There are two types of components - Class-based and Functional Components.

1. Class Components

   ```
   class MyComponent extends React.Component {
      constructor() {
        super();
        this.state = {
          key: "value"
        };
      };
      render() {
        return <div>...</div>;
      }
   }
   ```

2. Functional Components

   ```
   function MyComponent() {
     const [myState, setMyState] = useState("");

     useEffect(() => {
       ...
     }, []);

     return <div>...</div>;
   }
   ```

### State :

The state is a built-in React object that is used to contain data or information about the component. A component's state can change over time; whenever it changes, the component re-renders.

- A state can be modified based on user action or network changes
- Every time the state of an object changes, React re-renders the component to the browser
- The state object is initialized in the constructor
- The state object can store multiple properties
- this.setState() is used to change the value of the state object
- setState() function performs a shallow merge between the new and the previous state

### Props :
