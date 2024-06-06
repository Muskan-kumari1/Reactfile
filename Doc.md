**React js**

> **Table** **of** **Content**
>
> Introduction to React
>
> Features of React
>
> How to install React
>
> React Components
> 
> What are the advantages of React
> 
> How React Works
>
> Introduction to JSX
> 
> The difference between JSX and HTML
>
> Embedding JavaScript in JSX
>
> Managing state in React 
>
> Handling user events in React
>
> What is State
>




1

> **Introduction** **to** **React**
>
> React(also known as React.js or React js)is a free and open-source front-end Javascript library for building user interfaces based on components.
> 
> it is maintained by Meta(for mely Facebook)and a community of individual developers and companies.
>
> React is a declarative, component based library that allows developers to build reusable UI components and It follows the Virtual DOM (Document Object Model) approach, which optimizes rendering performance by minimizing DOM updates. React is fast and works well with other tools and libraries.
> 



2

> **Features of React**
>
> 

3








> **How** **to** **install** **React**
>
> There are a few different ways to install React.
>
> To start with, I highly recommend one approach, and that's using the
> officially recommended tool called
>
> create-react-app .
>
> create-react-app is a command line application, aimed at getting you
> up to speed with React in no time.
>
> You start by using npx , which is an easy way to download and execute
> Node.js commands without installing them.
>
> See my npx guide here: <https://flaviocopes.com/npx/>
>
> npx comes with npm (since version 5.2) and if you don't have npm
> installed already, do it now from
> [https://nodejs.org](https://nodejs.org/) (npm is installed with
> Node).
>
> If you are unsure which version of npm you have, run npm -v to check
> if you need to update.
>
> Tip: check out my OSX terminal tutorial at
> <https://flaviocopes.com/macos-terminal/> if you're unfamiliar with
> using the terminal, applies to Mac and Linux.
>
> When you run npx create-react-app \<app-name\> , npx is going to
> *download* the most recent create-react-app release, run it, and then
> remove it from your system. This is great because you will never have
> an

7
> **Advantages of React**
> 
The advantages of React JS are :

> It is composable.
> It is declarative.
> Write once, and learn anywhere.
> It is simple.
> SEO friendly.
> Fast, efficient, and easy to learn.
> It guarantees stable code.
> It is backed by a strong community.

8

<img src="./yjbifgkc.png"
style="width:4.53376in;height:5.09657in" />

||
||
||
||
||

> a [Git](https://flaviocopes.com/git/) repository.
>
> It also added a few commands in the package.json file:
>
> so you can immediately start the app by going into the newly created
> application folder and run npm start .

9

<img src="./vt5adbgg.png"
style="width:4.53376in;height:2.6473in" /><img src="./bhwpk5jf.png"
style="width:4.53376in;height:4.75263in" />

> By default this command launches the app on your local port 3000, and
> it opens your browser showing you the welcome screen:
>
> Now you're ready to work on this application!

10

> **React** **Components**
>
> You just saw how to create your first React application.
>
> This application comes with a series of files that do various things,
> mostly related to configuration, but there's one file that stands out:
> App.js .
>
> App.js is the **first** **React** **Component** you meet.
>
> Its code is this:
>
> <img src="./gampczne.png"
> style="width:4.58587in;height:0.20845in" />import React from 'react'
> import logo from './logo.svg' import './App.css'
>
> function App() { return (
>
> \<div className="App"\>
>
> \<header className="App-header"\>
>
> \<img src={logo} className="App-logo" alt="lo \<p\>
>
> Edit \<code\>src/App.js\</code\> and save to r \</p\>
>
> \<a
>
> className="App-link" href="https://reactjs.org" target="\_blank"
> rel="noopener noreferrer"
>
> \>
>
> Learn React \</a\>
>
> \</header\> \</div\>
>
> ) }
>
> export default App

11

> An application built using React, or one of the other popular frontend
> frameworks like Vue and Svelte for example, is built using dozens of
> components.
>
> But let's start by analyzing this first component. I'm going to
> simplify this component code like this:
>
> import React from 'react' import logo from './logo.svg' import
> './App.css'
>
> function App() {
>
> return /\* something \*/ }
>
> export default App
>
> You can see a few things here. We *import* some things, and we
> *export* a function called App .
>
> The things we import in this case are a JavaScript library (the react
> npm package), an SVG image, and a CSS file.
>
> create-react-app is set up in a way that allows us to import images
> and CSS to use in our JavaScript, but this is not something you need
> to care now. What you need to care about is the concept of a
> **component**
>
> App is a function that in the original example returns something that
> at first sight looks quite strange.
>
> It looks like **HTML** but it has some JavaScript embedded into it.

12

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

13

> **Introduction** **to** **JSX**
>
> We can't talk about React without first explaining JSX.
>
> You met your first React component, the App component defined in the
> default application built by
>
> create-react-app .
>
> Its code was this:
>
> <img src="./kvqmfprv.png"
> style="width:4.58587in;height:0.20845in" />import React from 'react'
> import logo from './logo.svg' import './App.css'
>
> function App() { return (
>
> \<div className="App"\>
>
> \<header className="App-header"\>
>
> \<img src={logo} className="App-logo" alt="lo \<p\>
>
> Edit \<code\>src/App.js\</code\> and save to r \</p\>
>
> \<a
>
> className="App-link" href="https://reactjs.org" target="\_blank"
> rel="noopener noreferrer"
>
> \>
>
> Learn React \</a\>
>
> \</header\>
>
> \</div\> )
>
> }
>
> export default App

14

> We previously ignored everything that was inside the

||
||
||

> talk about it.
>
> We call JSX everything inside wrapped inside the parentheses returned
> by the component:
>
> <img src="./bct1kpvg.png"
> style="width:4.58587in;height:0.20845in" />\<div className="App"\>
>
> \<header className="App-header"\>
>
> \<img src={logo} className="App-logo" alt="logo" \<p\>
>
> Edit \<code\>src/App.js\</code\> and save to reloa \</p\>
>
> \<a
>
> className="App-link" href="https://reactjs.org" target="\_blank"
> rel="noopener noreferrer"
>
> \>
>
> Learn React \</a\>
>
> \</header\> \</div\>
>
> This *looks* like HTML, but it's not really HTML. It's a little
> different.
>
> And it's a bit strange to have this code inside a JavaScript file.
> This does not look like JavaScript at all!
>
> Under the hood, React will process the JSX and it will transform it
> into JavaScript that the browser will be able to interpret.
>
> So we're writing JSX, but in the end there's a translation step that
> makes it digestible to a JavaScript interpreter.

15

> React gives us this interface for one reason: **it's** **easier**
> **to** **build** **UI** **interfaces** **using** **JSX**.
>
> Once you'll get more familiar with it, of course.
>
> In the next section we'll talk about how JSX lets you easily compose a
> UI, then we'll look at the differences with "normal HTML" that you
> need to know.

16

> **Using** **JSX** **to** **compose** **UI**
>
> As introduced in the last section, one of the main benefits of JSX is
> to make it very easy to build a UI.
>
> In particular, in a React component you can import other React
> components, and you can embed them and display them.
>
> A React component is usually created in its own file, because that's
> how we can easily reuse it (by importing it) in other components.
>
> But a React component can also be created in the same file of another
> component, if you plan to only use it in that component. There's no
> "rule" here, you can do what feels best to you.
>
> I generally use separate files when the number of lines in a file
> grows too much.
>
> To keep things simple let's create a component in the same App.js
> file.
>
> We're going to create a WelcomeMessage component:
>
> function WelcomeMessage() { return \<p\>Welcome!\</p\>
>
> }
>
> See? It's a simple function that returns a line of JSX that represents
> a p HTML element.
>
> We're going to add it to the App.js file.

17

||
||
||
||
||

> user interface:
>
> <img src="./wuhdnkad.png"
> style="width:4.58587in;height:0.20845in" />import React from 'react'
> import logo from './logo.svg' import './App.css'
>
> function WelcomeMessage() { return \<p\>Welcome!\</p\>
>
> }
>
> function App() { return (
>
> \<div className="App"\>
>
> \<header className="App-header"\>
>
> \<img src={logo} className="App-logo" alt="lo \<p\>
>
> Edit \<code\>src/App.js\</code\> and save to r \</p\>
>
> \<WelcomeMessage /\> \<a
>
> className="App-link" href="https://reactjs.org" target="\_blank"
> rel="noopener noreferrer"
>
> \>
>
> Learn React \</a\>
>
> \</header\> \</div\>
>
> ) }
>
> export default App
>
> And here's the result. Can you see the "Welcome!" message in the
> screen?

18

<img src="./cngllfo1.png"
style="width:4.53376in;height:3.56448in" />

> We say WelcomeMessage is a **child** **component** of App, and App is
> its parent componnet.
>
> We're adding the \<WelcomeMessage /\> component like if it was part of
> the HTML language.
>
> That's the beauty of React components and JSX: we can compose an
> application interface and use it like we're writing HTML.
>
> With some differences, as we'll see in the next section.

19

> **The** **difference** **between** **JSX** **and** **HTML**
>
> JSX kind of looks like HTML, but it's not.
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

20

<img src="./wdxmrbpw.png"
style="width:4.53376in;height:0.91718in" />

> React will try its best to make sure things don't break, but it will
> raise you a lot of warnings in the Developer Tools:
>
> This is not the only HTML feature that suffers from this problem, but
> it's the most common one.
>
> Another big difference between JSX and HTML is that HTML is very
> *relaxed*, we can say. Even if you have an error in the syntax, or you
> close the wrong tag, or you have a mismatch, the browser will try its
> best to interpret the HTML without breaking.
>
> It's one of the core features of the Web. It is very forgiving.
>
> JSX is not forgiving. If you forget to close a tag, you will have a
> clear error message:

21

<img src="./0kjvriks.png"
style="width:4.53376in;height:4.6901in" />

> React usually gives very good and informative error messages that
> point you in the right direction to fix the problem.
>
> Another big difference between JSX and HTML is that in JSX we can
> embed JavaScript.
>
> Let's talk about this in the next section.

22

> **Embedding** **JavaScript** **in** **JSX**
>
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

23

> We can print this value in the JSX by adding

||
||
||

> Inside the curly brackets { } we can add any JavaScript statement, but
> *just* *one* statement for every curly bracket block.
>
> And the statement must return something.
>
> For example this is a common statement you will find in JSX. We have a
> ternary operator where we define a condition ( message === 'Hello!' ),
> and we print one value if the condition is true, or another value (the
> content of message in this case) if the condition is false:
>
> <img src="./ykfnttkb.png"
> style="width:4.58587in;height:0.20845in" />{
>
> message === 'Hello!' ? 'The message was "Hello!"' }

24

> **Managing** **state** **in** **React**
>
> Every React component can have its own **state**.
>
> What do we mean by *state*? The state is the **set** **of** **data**
> **that** **is** **managed** **by** **the** **component**.
>
> Think about a form, for example. Each individual input element of the
> form is responsible for managing its state: what is written inside it.
>
> A button is responsible for knowing if it's being clicked, or not. If
> it's on focus.
>
> A link is responsible for knowing if the mouse is hovering it.
>
> In React, or in any other components-based framework/library, all our
> applications are based and make heavy use of components state.
>
> We manage state using the useState utility provided by React. It's
> technically a **hook** (you don't need to know the details of hooks
> right now, but that's what it is).
>
> You import useState from React in this way:
>
> import React, { useState } from 'react'
>
> Calling useState() , you will get back a new state variable, an a
> function that we can call to alter its value.

25

||
||
||

> and returns an array containing the state variable, and the function
> you call to alter the state.
>
> Example:
>
> const \[count, setCount\] = useState(0)
>
> This is important. We can't just alter the value of a state variable
> directly. We must call its modifier function. Otherwise the React
> component will not update its UI to reflect the changes of the data.
> Calling the modifier is the way we can tell React that the component
> state has changed.
>
> The syntax is a bit weird, right? Since useState() returns an array we
> use array destructuring to access each individual item, like this:
> const \[count, setCount\] = useState(0)
>
> Here's a practical example:
>
> <img src="./vy4wr1p5.png"
> style="width:4.58587in;height:0.20845in" />import { useState } from
> 'react'
>
> const Counter = () =\> {
>
> const \[count, setCount\] = useState(0)
>
> return ( \<div\>
>
> \<p\>You clicked {count} times\</p\>
>
> \<button onClick={() =\> setCount(count + 1)}\>Cl \</div\>
>
> ) }
>
> ReactDOM.render(\<Counter /\>, document.getElementById

26

||
||
||

> create as many state variables as you want:
>
> <img src="./ly5p4dno.png"
> style="width:4.58587in;height:0.20845in" />const \[count, setCount\] =
> useState(0)
>
> const \[anotherCounter, setAnotherCounter\] = useState

27

> **Component** **Props** **in** **React**
>
> We call props the initial values passed to a component.
>
> We previously created a WelcomeMessage component
>
> function WelcomeMessage() { return \<p\>Welcome!\</p\>
>
> }
>
> and we used it like this:
>
> \<WelcomeMessage /\>
>
> This component does not have any initial value. It does not have
> props.
>
> Props can be passed as attributes to the component in the JSX:
>
> \<WelcomeMessage myprop={'somevalue'} /\>
>
> and inside the component we receive the props as argument:
>
> function WelcomeMessage(props) { return \<p\>Welcome!\</p\>
>
> }

28

> It's common to use object destructuring to get the props by name:
>
> function WelcomeMessage({ myprop }) { return \<p\>Welcome!\</p\>
>
> }
>
> Now that we have the prop, we can use it inside the component, for
> example we can print its value in the JSX:
>
> function WelcomeMessage({ myprop }) { return \<p\>{myprop}\</p\>
>
> }
>
> Curly brackets here have various meanings. In the case of the function
> argument, curly brackets are used as part of the object destructuring
> syntax.
>
> Then we use them to define the function code block, and finally in the
> JSX to print the JavaScript value.
>
> Passing props to components is a great way to pass values around in
> your application.
>
> A component either holds data (has state) or receives data through its
> props.
>
> We can also send functions as props, so a child component can call a
> function in the parent component.
>
> A special prop is called children . That contains the value of
> anything that is passed between the opening and closing tags of the
> component, for example:

29

<img src="./5xnps50w.png"
style="width:4.58587in;height:0.20845in" />

> In this case, inside WelcomeMessage we could access the value Here is
> some message by using the
>
> children prop:
>
> function WelcomeMessage({ children }) { return \<p\>{children}\</p\>
>
> }

30

> **Data** **flow** **in** **a** **React** **application**
>
> In a React application, data typically flows from a parent component
> to a child component, using props as we saw in the previous section:
>
> \<WelcomeMessage myprop={'somevalue'} /\>
>
> If you pass a function to the child component, you can however change
> the state of the parent component from a child component:
>
> const \[count, setCount\] = useState(0)
>
> \<Counter setCount={setCount} /\>
>
> Inside the Counter component we can now grab the setCount prop and
> call it to update the count state
>
> in the parent component, when something happens:
>
> function Counter({ setCount }) { //...
>
> setCount(1)
>
> //... }
>
> You need to know that there are more advanced ways to manage data,
> which include the Context API and libraries like Redux, but those
> introduce more

31

> complexity and 90% of the times using those 2 ways I just explained
> are the perfect solution.

32

> **Handling** **user** **events** **in** **React**
>
> React provides an easy way to manage events fired from DOM events like
> clicks, form events and more.
>
> Let's talk about click events, which are pretty simple to digest.
>
> You can use the onClick attribute on any JSX element:
>
> \<button onClick={(event) =\> {
>
> /\* handle the event \*/ }}
>
> \>
>
> Click here \</button\>
>
> When the element is clicked, the function passed to the onClick
> attribute is fired.
>
> You can define this function outside of the JSX:
>
> <img src="./4lsln2zv.png"
> style="width:4.58587in;height:0.20845in" />const handleClickEvent =
> (event) =\> { /\* handle the event \*/
>
> }
>
> function App() {
>
> return \<button onClick={handleClickEvent}\>Click he }
>
> When the click event is fired on the button, React calls the event
> handler function.

33

> React supports a vast amount of types of events, like

||
||
||

> onSubmit and many more.

34

> **Lifecycle** **events** **in** **a** **React** **component**
>
> So far we've seen how to manage state with the useState hook.
>
> There's another hook I want to introduce in this book: useEffect .
>
> The useEffect hook allows components to have access to the lifecycle
> events of a component.
>
> When you call the hook, you pass it a function. The function will be
> run by React when the component is first rendered, and on every
> subsequent re-render/update.
>
> React first updates the DOM, then calls any function passed to
> useEffect() .
>
> All without blocking the UI rendering even on blocking code.
>
> Here is an example:

35

<img src="./4ionaaaz.png"
style="width:4.58587in;height:0.20845in" />

> Since the useEffect() function is run on every subsequent
> re-render/update of the component, we can tell React to skip it, for
> performance purposes, by adding a second parameter which is an array
> that contains a list of state variables to watch for. React will only
> re-run the side effect if one of the items in this array changes.
>
> <img src="./2wnftuz2.png"
> style="width:4.58587in;height:0.20845in" />useEffect(() =\> {
>
> console.log(\`Hi \${name} you clicked \${count} times }, \[name,
> count\])
>
> Similarly, you can tell React to only execute the side effect once (at
> mount time), by passing an empty array:
>
> useEffect(() =\> { console.log(\`Component mounted\`)
>
> }, \[\])

36

> You migth find yourself using this option a lot.
>
> useEffect() is great for adding logs, accessing 3rd party APIs and
> much more.

37

> **Where** **to** **go** **from** **here**
>
> Mastering the topics explained in this book is a great step towards
> your goal of learning React.
>
> I want to give you some pointers now, because it's easy to get lost in
> the sea of tutorials and courses about React.
>
> What should you learn next?
>
> [Learn more theory about the Virtual DOM,
> writing](https://flaviocopes.com/react-declarative/) [declarative
> code,](https://flaviocopes.com/react-declarative/) [unidirectional
> data flow,](https://flaviocopes.com/react-unidirectional-data-flow/)
> [immutability,](https://flaviocopes.com/react-immutability/)
> [composition.](https://flaviocopes.com/react-composition/)
>
> Start building some simple React applications. For [example build a
> simple counter or a interact with
> a](https://flaviocopes.com/react-example-githubusers/) [public
> API.](https://flaviocopes.com/react-example-githubusers/)
>
> Learn how to perform [conditional
> rendering,](https://flaviocopes.com/react-conditional-rendering/) how
> to [perform loops in JSX, how to use the React
> Developer](https://flaviocopes.com/react-developer-tools/)
> [Tools.](https://flaviocopes.com/react-developer-tools/)
>
> Learn how to apply CSS in a React application, with [plain
> CSS](https://flaviocopes.com/react-css/) or [Styled
> Components.](https://flaviocopes.com/styled-components/)
>
> Learn how to manage state using the [Context
> API,](https://flaviocopes.com/react-context-api/) useContext and
> [Redux.](https://flaviocopes.com/redux/)
>
> Learn how to interact with
> [forms.](https://flaviocopes.com/react-forms/)
>
> Learn how to use [React
> Router.](https://flaviocopes.com/react-router/)
>
> Learn [how to test React
> applications.](https://flaviocopes.com/react-testing-components/)
>
> Learn an application framework built on top of React,

<u>like</u> [<u>Gatsby</u>](https://flaviocopes.com/gatsby/) <u>or
[Next.js.](https://flaviocopes.com/nextjs/)</u>

38

> Most of all, make sure you practice by building sample applications to
> apply everything you learn.

39
