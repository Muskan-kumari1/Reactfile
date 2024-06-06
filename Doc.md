# React js

![image](https://media.dev.to/cdn-cgi/image/width=750,height=700,fit=cover,gravity=auto,format=auto/https%3A%2F%2Fdev-to-uploads.s3.amazonaws.com%2Fuploads%2Farticles%2F096baapsqqt9fks0us99.png)


### Table of Content

1. Introduction to React

2. Features of React

3. How to install React

4. React Components

5. What are the advantages of React
 
6. How React Works

7. Introduction to JSX

8. The difference between JSX and HTML

9. Embedding JavaScript in JSX

10. Managing state in React 

11. Handling user events in React

12. Understanding React js Props. What is "Props"?


## 1. Introduction to React

 * React(also known as React.js or React js)is a free and open-source front-end Javascript library for building user interfaces based on components.
 
 * it is maintained by Meta(for mely Facebook)and a community of individual developers and companies.

 * React is a declarative, component based library that allows developers to build reusable UI components and It follows the Virtual DOM (Document Object Model) approach, which optimizes rendering performance by minimizing DOM updates. React is fast and works well with other tools and libraries.
 

## 2.Features of React

 JSX(JavaScript Syntax Extension):
 
 Virtual DOM:
 
 One-way Data Binding:
 
 Performance:
 
 Extension:
 
 Conditional Statements:
 
 Components:
 
 Simplicity: 


## 3. How to install React
> There are a few different ways to install React.
> To start with, I highly recommend one approach, and that's using the
> officially recommended tool called

> create-react-app .

> create-react-app is a command line application, aimed at getting you
> up to speed with React in no time.

> You start by using npx , which is an easy way to download and execute
> Node.js commands without installing them.

> See my npx guide here: <https://flaviocopes.com/npx/>

> npx comes with npm (since version 5.2) and if you don't have npm
> installed already, do it now from
> [https://nodejs.org](https://nodejs.org/) (npm is installed with
> Node).

> If you are unsure which version of npm you have, run npm -v to check
> if you need to update.
>
> Tip: check out my OSX terminal tutorial at
> <https://flaviocopes.com/macos-terminal/> if you're unfamiliar with
> using the terminal, applies to Mac and Linux.

> When you run npx create-react-app \<app-name\> , npx is going to
> *download* the most recent create-react-app release, run it, and then
> remove it from your system. This is great because you will never have
> an

## 4. React Components

> components are independent and reusable bits of code.

> Componenets are Javascript files.
> They Serve the some purpose as Javascript functions.
>
> But works in isolation and returns HTML via a render function.

 ```bash
<img src="./gampczne.png"
 style="width:4.58587in;height:0.20845in" />import React from 'react'
 import logo from './logo.svg' import './App.css'

 function App() { return (

 \<div className="App"\>

 \<header className="App-header"\>

 \<img src={logo} className="App-logo" alt="lo \<p\>

 Edit \<code\>src/App.js\</code\> and save to r \</p\>

 \<a

 className="App-link" href="https://reactjs.org" target="\_blank"
rel="noopener noreferrer"

 \>
 Learn React \</a\>
 
 \</header\> \</div\>

 ) }
export default App
```


## 5. Advantages of React

* The advantages of React JS are :

*  It is composable.
 
*  t is declarative.
 
* Write once, and learn anywhere.
 
* It is simple.
 
* SEO friendly.
 
* Fast, efficient, and easy to learn.
 
* It guarantees stable code.
 
* It is backed by a strong community.

## 6. How React Works
* `Component-Based Architecture:` React structures applications using components. These are self-contained, reusable pieces of UI that can be nested, managed, and handled independently. Each component can have its own state and lifecycle.
* `JSX Syntax:` React uses JSX, a syntax extension for JavaScript, which allows developers to write HTML-like code within JavaScript. This makes the code more readable and easier to write.
* `Virtual DOM:` React maintains a virtual representation of the DOM in memory. When the state of a component changes, React updates the virtual DOM first. It then compares this virtual DOM with the actual DOM and determines the most efficient way to update the actual DOM to match the virtual one. This process is called reconciliation.
* `State and Props:` Components in React can hold their own state, which is used to manage data that changes over time. Props (short for properties) are used to pass data from parent components to child components. This unidirectional data flow ensures predictable data management.
* `Lifecycle Methods:` React components have a lifecycle, and developers can hook into different stages of this lifecycle using methods like componentDidMount, componentDidUpdate, and componentWillUnmount. These methods provide opportunities to execute code at specific points in a component's life.
* `Hooks:` Introduced in React 16.8, hooks allow developers to use state and other React features in functional components. Common hooks include useState for managing state and useEffect for handling side effects.
* React Router: For building single-page applications, React Router is often used to manage navigation and rendering of different components based on the URL.


## 7. Introductions to JSX


> JSX stands for JavaScript XML. JSX is basically a syntax extension of JavaScript.
> 
> React JSX helps us to write HTML in JavaScript and forms the basis of React Development.
> 
> Using JSX is not compulsory but it is highly recommended for programming in React as it makes the  >development process easier as the code becomes easy to write and read.

**We can't talk about React without first explaining JSX.
 You met your first React component, the App component defined in the
default application built by  `create-react-app.`

 **Its code was this:**
```bash
 <img src="./kvqmfprv.png"
 style="width:4.58587in;height:0.20845in" />import React from 'react'
 import logo from './logo.svg' import './App.css'

 function App() { return (

 \<div className="App"\>

 \<header className="App-header"\>

 \<img src={logo} className="App-logo" alt="lo \<p\>

 Edit \<code\>src/App.js\</code\> and save to r \</p\>

 \<a

 className="App-link" href="https://reactjs.org" target="\_blank"
 rel="noopener noreferrer"

 \>

 Learn React \</a\>

 \</header\>

 \</div\> )

 }

 export default App
 ```

## 8. The difference between JSX and HTML

 JSX kind of looks like HTML, but it's not.
>
> In this section I want to introduce you some of the most important
> things you need to keep in mind when using JSX.
>
> One of the differences might be quite obvious if you looked at the App
> component JSX: there's a strange attribute called className .
>
> In HTML we use the class attribute. It's probably the most widely used
> attribute, for various reasons. One of those reasons is CSS. The class
> attribute allows us to style HTML elements easily, and CSS frameworks
> like Tailwind put this attribute to the center of the CSS user
> interface design process.
>
> But there's a problem. We are writing this UI code in a JavaScript
> file, and class in the JavaScript programming language is a reserved
> word. This means we can't use this reserved word as we want. It serves
> a specific purpose (defining JavaScript classes) and the React
> creators had to choose a different name for it.
>
> That's how we ended up with className instead of class .
>
> You need to remember this especially when you're copy/pasting some
> existing HTML.


> That is **JSX**, a special language we use to build a component's
> output. We'll talk more about JSX in the next section.
>
> In addition to defining some JSX to return, a component has several
> other characteristics.
>
> A component can have its own **state**, which means it encapsulates
> some variables that other components can't access unless this
> component exposes this state to the rest of the application.
>
> A component can also receive data from other components. In this case
> we talk about **props**.
>
> Don't worry, we're going to look in details at all those terms (JSX,
> State and Props) soon.

## 9. Embedding JavaScript in JSX

> One of the best features of React is that we can easily embed
> JavaScript into JSX.
>
> Other frontend frameworks, for example Angular and Vue, have their own
> specific ways to print JavaScript values in the template, or perform
> things like loops.
>
> React is not adding new things. Instead, it lets us use JavaScript in
> the JSX, by using curly brackets.
>
> The first example of this that I will show you comes directly from the
> App component we studied so far.
>
> We import the logo SVG file using
>
> import logo from './logo.svg'
>
> and then in the JSX we assign this SVG file to the src attribute of an
> img tag:
>
> \<img src={logo} class="App-logo" alt="logo" /\>
>
> Let's do another example. Suppose the App component has a variable
> called message :
>
> function App() {
>
> const message = 'Hello!' //...
>
> }

## 10. Managing state in React 

* Component State: State is a built-in React object used to hold data that can change over time. Each class component can have its own state, initialized in the constructor, and updated using this.setState(). Functional components use the useState hook to handle state.

* useState Hook: For functional components, the useState hook is used to declare state variables. It returns an array with two elements: the current state value and a function to update it. This hook allows functional components to have state and manage it.

* Props for State Passing: State can be passed from parent to child components via props. This enables child components to access and display state data from their parents, promoting a unidirectional data flow.

* State Libraries: For larger applications, state management libraries like Redux, MobX, or Zustand are used. These libraries provide a more structured and scalable approach to handling state across an entire application, offering features like centralized state, middleware, and time-travel debugging.

```bash
import React, { Component } from 'react';

class Counter extends Component {
  constructor(props) {
    super(props);
    this.state = { count: 0 };
  }

  increment = () => {
    this.setState({ count: this.state.count + 1 });
  };

  render() {
    return (
      <div>
        <p>Count: {this.state.count}</p>
        <button onClick={this.increment}>Increment</button>
      </div>
    );
  }
}

export default Counter;
```

## 11. Handling user events in React

**Handling user events in React involves setting up event handlers that respond to user actions like clicks, keyboard input, or form submissions. Here’s a brief description of how to manage user events in React:**

* Event Handlers: React uses camelCase for event handler properties, such as onClick, onChange, onSubmit, etc. These handlers are functions defined either as class methods or within functional components.

* Binding Event Handlers: In class components, event handler methods often need to be bound to the component instance to ensure the correct this context. This can be done using the .bind() method in the constructor or by using arrow functions.

* Passing Arguments: To pass arguments to event handlers, you can use an arrow function or the .bind() method within the JSX. This ensures the handler receives the necessary parameters when the event occurs.

* Preventing Default Behavior: To prevent the default behavior of an event (like form submission), you can call event.preventDefault() within the event handler.

* Synthetic Events: React uses synthetic events, which are a cross-browser wrapper around the browser's native event system. This ensures consistent behavior across different browsers.

* State Updates: Event handlers often update the component’s state using this.setState() in class components or the setState function in functional components. This triggers a re-render, updating the UI in response to the user action.

```bash
import React, { Component } from 'react';

class ClickButton extends Component {
  constructor(props) {
    super(props);
    this.state = { count: 0 };
    this.handleClick = this.handleClick.bind(this);
  }

  handleClick() {
    this.setState({ count: this.state.count + 1 });
  }

  render() {
    return (
      <div>
        <p>Count: {this.state.count}</p>
        <button onClick={this.handleClick}>Click Me</button>
      </div>
    );
  }
}

export default ClickButton;

`Functional Component Handling a Click Event`
```
```bash
import React, { useState } from 'react';

const ClickButton = () => {
  const [count, setCount] = useState(0);

  const handleClick = () => {
    setCount(count + 1);
  };

  return (
    <div>
      <p>Count: {count}</p>
      <button onClick={handleClick}>Click Me</button>
    </div>
  );
};

export default ClickButton;

```

## 12. Understanding React js Props. What is "Props"?

* 
In React, "props" (short for properties) are a mechanism for passing data from a parent component to a child component. Props are used to customize and configure child components, enabling the creation of reusable and dynamic UI components. Here’s an overview of how props work:

**What Are Props?**

* Data Passing: Props allow you to pass data from a parent component to a child component. This data can be of any type: strings, numbers, arrays, objects, functions, etc.

* Read-Only: Props are immutable, meaning they cannot be modified by the child component. This ensures a unidirectional data flow, promoting a clear and predictable structure in your application.

* Attributes in JSX: Props are passed to child components similarly to how attributes are added to HTML elements. They are specified within the JSX tags of the child component.

**How to Use Props**
```bash
<ChildComponent name="John" age={30} />
```

**Accessing Props: In the child component, props can be accessed via this.props in class components or directly as a function parameter in functional components.**

```bash
// Class Component
class ChildComponent extends React.Component {
  render() {
    return (
      <div>
        <p>Name: {this.props.name}</p>
        <p>Age: {this.props.age}</p>
      </div>
    );
  }
}

// Functional Component
const ChildComponent = (props) => {
  return (
    <div>
      <p>Name: {props.name}</p>
      <p>Age: {props.age}</p>
    </div>
  );
};

```

**Default Props: You can define default values for props in case they are not provided by the parent component.**
```bash
ChildComponent.defaultProps = {
  name: 'Unknown',
  age: 0
};

```



**Parent Component**

```bash
import React from 'react';
import ChildComponent from './ChildComponent';

const ParentComponent = () => {
  return (
    <div>
      <ChildComponent name="John" age={30} />
      <ChildComponent name="Jane" age={25} />
    </div>
  );
};

export default ParentComponent;
```

**Child Component**
```bash
import React from 'react';

// Functional Component
const ChildComponent = (props) => {
  return (
    <div>
      <p>Name: {props.name}</p>
      <p>Age: {props.age}</p>
    </div>
  );
};

// Setting default props
ChildComponent.defaultProps = {
  name: 'Unknown',
  age: 0
};

export default ChildComponent;

```
### Thank You!

