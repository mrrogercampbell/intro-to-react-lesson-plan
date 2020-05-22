# Intro to React
![](name-of-giphy.gif)
# Instructor Prep Section
This section provides instructors extra details on the break down of this lesson.

## Legend
- **I Do** - Instructor-led demos
    - Students should **not** code along
- **We Do** - Instructor-led demos
    - Students should code along
- **You Do** - Test for understanding
    - Students should complete on their own
    - They can ask for instructor assistance
- **Cold Call** - Instructor calls on a random student(s) to answer prompt(s)
- **Turn and Discuss** - Student-led dialogue
    - Have students turn to their neighbor(s) and discuss the provided prompts
    - If time permits:
        - Once time allotted has lapsed the instructor should call on each group and have a representative talk about what their group discussed
- **Breakout Groups** - Break students into small groups to work through provided prompts
    - Typically 10-15 min time blocks

## Delivery Tips
<details>
<summary>Click here</summary>
<br>
<ul>
  <li>Think about how long you&#39;re talking</li>
  <li>Move quicker sooner, slower later</li>
  <li>Cold Call more often</li>
  <li>Revisit Learning Objects</li>
  <li>Defer questions when appropriate</li>
</ul>
</details>


## Prep Resources
This section is meant to provide instructor helpful links that will assist them in preparing to teach this lesson. It should contain any resources that Curriculum Engineers used to write the lesson.
<details>
<summary>Click Here</summary>
<br>
<ul>
  <li><a href="https://reactjs.org/docs/getting-started.html">React Documentation</a></li>
  <li><a href="https://reactjs.org/tutorial/tutorial.html">React Docs: Tutorial - Intro to React</a></li>
  <li><a href="https://www.w3schools.com/react/">W3Schools: React Tutorial</a></li>
  <li><a href="https://scotch.io/starters/react/getting-started-with-react-2019-edition">Scotch.io: Getting Started with React</a></li>
  <li><a href="https://www.codecademy.com/articles/react-virtual-dom">React: The Virtual DOM</a></li>
  <li><a href="https://www.lullabot.com/articles/how-to-learn-react">How to Learn React: A Five-Step Plan</a></li>
  <li><a href="https://medium.com/@baphemot/a-react-job-interview-recruiter-perspective-f1096f54dd16">A React Job Interview - Recruiter Perspective</a></li>
</ul>

</details>

# Table of Content
- [Intro to React](#intro-to-react)
- [Instructor Prep Section](#instructor-prep-section)
  - [Legend](#legend)
  - [Delivery Tips](#delivery-tips)
  - [Prep Resources](#prep-resources)
- [Table of Content](#table-of-content)
- [Lesson Outline](#lesson-outline)
  - [Prerequisites](#prerequisites)
  - [Learning Objectives](#learning-objectives)
  - [Thinking in React](#thinking-in-react)
    - [What is a framework?](#what-is-a-framework)
    - [DOM Manipulation in Vanilla JavaScript](#dom-manipulation-in-vanilla-javascript)
    - [Vanilla JS DOM Manipulation Review: Cold Call or Breakout Groups](#vanilla-js-dom-manipulation-review-cold-call-or-breakout-groups)
    - [The Virtual DOM](#the-virtual-dom)
    - [JSX](#jsx)
  - [Components](#components)
    - [Functional Components](#functional-components)
    - [Your First Component: We Do](#your-first-component-we-do)
    - [Class Components](#class-components)
    - [Your Second Component: We Do](#your-second-component-we-do)
    - [Class vs Functional](#class-vs-functional)
    - [Build Two Components: You Do](#build-two-components-you-do)
  - [Props and State](#props-and-state)
    - [Props](#props)
    - [Rendering Props: I Do](#rendering-props-i-do)
    - [State](#state)
    - [Rendering State: I Do](#rendering-state-i-do)
    - [Passing State and Rendering State: I Do](#passing-state-and-rendering-state-i-do)
    - [How Do You Conceptualize Props and State: Turn and Discuss](#how-do-you-conceptualize-props-and-state-turn-and-discuss)
  - [Check for Understanding](#check-for-understanding)
- [Survey and Feedback](#survey-and-feedback)

# Lesson Outline

## Prerequisites
* JavaScript Fundamentals
* Understanding of OOP
* Basic Data Types

## Learning Objectives
- By the end of this lesson students should be able to:
    - Define what React is and why it is used
    - Explain what JSX is and how it is utilized within the context of a React project
    - Be able to discuss and understand the following React concepts:
        - Rendering Elements with JSX
        - Purpose of React `Functional` and `Class` components
    - Build basic React components that can:
        - Instantiate, render, and manipulate `state`
        - Pass `state` and `props` into a child component
        - Render `props` that have been passed to it
    - Explain the difference between:
        - Props and State
        - Class and Function Components
    - Be able to define and discuss all words in the `Vocabulary` section below

## Thinking in React
This section gives an overview of the principals of React and how to conceptualize utilizing it while designing and building applications.
- Key Takeaways:
	- How React allows you to modularize `Encapsulation`
	- Review `Separation of Concerns` and how it is redesigned within React

### What is a framework?
Section intro which allows the instructor to explain/review the concept of a framework.
- Key Takeaways:
	- The difference between a `framework` and a `library`
	- The fact that React is commonly misconceived as a `framework` when in fact it is a JavaScript `library`
### DOM Manipulation in Vanilla JavaScript
A quick review on `DOM manipulation` which will explain the complication you encounter when using DOM manipulation in vanilla JavaScript when dealing with an enterprise-size application

### Vanilla JS DOM Manipulation Review: Cold Call or Breakout Groups

Depending on class size use one of the following:
1. Call on a random student for each of the following prompts and have them provide you the code solution.
2. Have students break into small groups (2-3 based off class size) and work through each prompt together.

**Prompts**:
- Create a variable which stores a DOM selector for:
	- The `h1` element with a class of `grab-me`
	- The `button` element with an `id` of `click-me`
- Define a function that adds a `click event` to the `click-me` button which changes the `innerText` of the selected `h1` element

Once they complete this, talk about how cumbersome `DOM Manipulation` can become when dealing with a larger application such as Twitter, Facebook, etc.

### The Virtual DOM
A quick introduction to the `virtual DOM`.

**Key Takeaways**:
- The `Virtual DOM` is a JavaScript `object` that represents the true `DOM structure`.
- The `Virtual DOM` allows us to make changes to the true DOM by first altering the virtual DOM, then it renders the changes for us.
- When you update the `DOM` in React:
	- The entire `virtual DOM` is updated and re-rendered
	- React can compare the `virtual DOM` previous state and see what changes were made
	- Only the changed objects are updated on the DOM
	- Changes on the real `DOM` are then displayed the screen

### JSX
Introduce students to `JSX`.

**Key Takeaways**:
- `JSX` is not `HTML`, it is a `JavaScript Syntax`
- `JSX` allows you to write concise `HTML` in `JavaScript` which `Babel` transforms into actual `JavaScript` code

## Components
An introduction to React `components`.

**Key Takeaways**:
- A React `Component` is a JavaScript `Class` or `Function` that allows you to develop independent and reusable bits of code
- Components have a similar use case as a JavaScript function, but work independently and return `JSX` via a render method which is compiled into `JavaScript` and `HTML`
- There are two types of components:
	1. `Class` components
	1. `Function` components

### Functional Components
This section gives an in-depth explanation of `functional` components.

**Key Takeaways**:
- A `functional` component is a basic JavaScript function
- Typically written as an arrow function
- They were considered `dumb` or `stateless` components because they were unable to utilize `React lifecycle` methods until the introduction of `React Hooks`
  - Touch on this but hold off on diving too far into `Hook`
    - They will be covered in a later lesson


### Your First Component: We Do
Walk students through writing out their first functional component.

 **Prompts**:
- Create a `functional` component called `Hello`
- It should render:
	- `h1` that says `Hello <provide a name of choice>, Welcome to <provide a class name>`

Example:
```JSX
import React from 'react'

const Mantra = () => {
    return (
      <div>
	      <h1>This is the Way!</h1>
      </div>
    )
}

export default Mantra
```

### Class Components
This section gives an in-depth explanation of `class` components.

**Key Takeaways**:
- `Class` components extend the ES6 JavaScript class `Component`
- `Class` components are considered a `smart` and or `stateful` components
- `Class` components are able to utilize `React lifecycle` methods

### Your Second Component: We Do
Walk students through converting the `functional` component they created in the last `We Do` into a class component.

**Prompts**:
- Create a `class` component called `Hello`
- It should render:
	- `h1` that says `Hello <provide a name of choice>, Welcome to <provide a class name>`

Example:
```JSX
import React from 'react'

class Hello extends React.Component {
  render() {
    return (
      <div>
	      <h1>Hello Spyro, Welcome to firefighting 101!  </h1>
      </div>
    )
  }
}
export default Hello
```

### Class vs Functional
A brief explanation of when to use which and the pain points associated with each.

**Key Takeaways**:
- At inception, the running rule was to use `Class components` when you wanted to utilize `state` and `Function components` when you just wanted to render static data and or data stored within `props`
- Yet with the introduction  of `React Hooks` that all went out the window
	- Facebook's official recommendation is to use `functional` components whenever possible
		- Although many Developers and Engineer debate this point

### Build Two Components: You Do
Have students create a `functional` and `class` component on their own.

**Prompts**:
1. Create a `class` component that:
   - Renders a `h1` that says `Hello, my name is <type-your-name-here>. I am from <type-the-name-of-hometown-here>`
2. Create a `functional` component that:
   - Renders a `h1` that says `Hello, my name is <type-your-name-here>. I am from <type-the-name-of-hometown-here>`

## Props and State
This section intro is an overview of what students will learn in the **Props** and **State** sections below.

**Key Takeaways**:
- React is a front end library
- It allows developers to rapidly build front end web applications
- React alleviates the heavy lift a developers has to do when working with Vanilla JavaScript, HTML, and CSS.

### Props
**Key Takeaways**:
- `Props` is short for `properties`
- `Props` are variables which store data
- `Props` are `immutable`, meaning their value can not be changed
- `Props` are passed into a component by its `parent` component

### Rendering Props: I Do
Demonstrate to students how to write a `Functional` and `Class` component which both render `props`.

Example:
```JSX
import React from "react";
import "./styles.css";

const Greeting = props => {
  return (
    <div>
      <h1>
        I am {props.name}.... I am {props.name}!
      </h1>
    </div>
  );
};

const App = props => {
  return (
    <div>
      <Greeting name={"Groot"} />
    </div>
  );
};

export default App;
```

### State
Key Takeaways:
- `State` is a JavaScript object which is defined in the constructor of a `Class component`
- `State`'s purpose is to hold data for a component
- You define variables within `state` which in turn can be accessed and rendered within a component
- A parent component can pass it's own `state` to a child component in the form a `prop`

### Rendering State: I Do
Build a `Class` component that renders `state`.

Example:
```jsx
import React from "react";
import "./styles.css";

class App extends React.Component {
  constructor() {
    super();
    this.state = {
      name: "Luke",
      class: "How to use a lightsaber while blindfolded"
    };
  }

  render() {
    return (
      <div>
        <h1>
          Hello {this.state.name}, Welcome to the course: {this.state.class}!
        </h1>
      </div>
    );
  }
}
export default App;

```

### Passing State and Rendering State: I Do

**Prompts**:
- Create a `function` component called `Hello`
	- It should expect to take in two `props`: `name` and `class`; it should then render them in the following sentence:
	- Hello <name-goes-here>, welcome to <class-goes-here>!
- Refactor your previously created the `App` `Class` component so that it:
	- Renders the `Hello` component as a child
	- Passes the `Hello` component the all the data stored within its `state`; ie: `name` and `class`

**Solution provided inside the lesson**

### How Do You Conceptualize Props and State: Turn and Discuss
Have student turn to their neighbor and discuss the following amongst themselves for 10 mins:
- How they conceptualize `props` and `state`
- What is the difference between `props` and `state`
- Talk about an instance within an application where they might need to pass `state` to another component
- When might they need to only use `props` within a component

Once 10 mins have elapsed, call on one group for each prompt, and have them explain what they discussed.

## Check for Understanding
This section is meant to provide multiple assessments that instructors can utilize to test and quantify student understanding of the lesson.

**Assessment Questions**:
1. Is React a `library` or a `framework`
3. When should you use a `function` component over a `class` component?
4. What is the difference between `props` and `state`?
5. How do you pass the `state` of one component to another?
6. Have each student in their own words define the following vocabulary words:
    - `Framework`
    - `library`
    - `Virtual DOM`
    - `JSX`
    - `Components`
    - `Functional Components`
    - `Class Components`
    - `Props`
    - `State`

# Survey and Feedback
The Curriculum team loves constructive and creative feedback. Please feel free to fill out this survey and [feedback](https://forms.gle/yaiUyN4YDSxFLp1s6) and we will do our best to accommodate your requests. and we will do our best to accommodate your requests.