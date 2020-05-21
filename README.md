# Intro to React

## Prerequisites
* JavaScript Fundamentals:
* Understanding with OOP
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

## Vocabulary

- `Framework`
- `library`
- `Virtual DOM`
- `JSX`
- `Components`
- `Functional Components`
- `Class Components`
- `Props`
- `State`

# Lesson Outline:

## Thinking in React
This section introduces students to the basic principals of React and how to conceptualize utilizing it while designing and building applications. A key point to touch on here is encapsulation.

### What is a framework?
Brief overview explaining:
- The difference between a `framework` and a `library`
- The fact that React is commonly misconceived as a `framework` when in fact it is a JavaScript `library`
### DOM Manipulation in Vanilla JavaScript
- Quick review on DOM manipulation
- Talk about the complication you encounter when using DOM manipulation in vanilla JavaScript when dealing with an enterprise-size application

### Vanilla JS DOM Manipulation Review - Cold Call || Breakout Groups
-  Starter code is provided within lesson repo
-  Call on a random student for each of the following prompts and have them provide you the code solution.
                OR
- Have students break into small groups (2-3 based off class size) and work through each prompt together
    - A variable which stores a DOM selector for:
       -  The `h1` element with a class of `grab-me`
       -  The `button` element with an `id` of `click-me`
       -  Define a function that adds a `click event` to the `click-me` button which changes the `innerText` of the selected `h1` element.

Once they complete this explain to them how cumbersome this can become with dealing with a larger application such as Twitter, Facebook, etc.


### The Virtual DOM
A quick intro to the virtual DOM. 
Main Takeaways:
- The `Virtual DOM` is a JavaScript `object` that represents the true `DOM structure`.
- The `Virtual DOM` allows us to make changes to the true DOM by first altering the virtual DOM, then it renders the changes for us. 

### JSX
Introduce students to `JSX`.
Main Takeaways:
- `JSX` is not `HTML`, it is a a `JavaScript Syntax`
- `JSX` allows you to write concise `HTML` in you `JavaScript` which `Babel` transforms into actual `JavaScript` code.

## Components
Introduce Students too `React Components` by walking them through coding 
Main Takeaways:
- A React `Component` is a JavaScript `Class` or `Function` that allow you to develop independent and reusable bits of code
- Have a similar use case as a JavaScript function, but work independently and return HTML via a render function
- There are two types of components:
	1. `Class` components:
	1. `Function` components:
		- Basis JavaScript functions
		- Typically arrow functions
		- Where considered `dumb` or `stateless` components and were unable to utilize `React lifecycle` methods until the introduction of `React Hooks`
			- Touch on this but hold off of diving to far in, this will be covered in a later lesson

### Functional Components
Something here
- Main Takeaways:
	- Basis JavaScript functions
	- Typically arrow functions
	- Where considered `dumb` or `stateless` components and were unable to utilize `React lifecycle` methods until the introduction of `React Hooks`
		- Touch on this but hold off of diving to far in, this will be covered in a later lesson


### Your First Component - **We Do**
Walk students through writing out their first functional component. 
**Prompt and code snippets provided in lesson**

### Class Components
- `Main Takeaways:
	- A JavaScript class which extends the `Component` class from ES6
	- Considered a `smart` and or `stateful` component
	- Able to utilizes `React lifecycle` methods

### Your Second Component - **We Do**
Walk students through writing out their first class component. 
**Prompt and code snippets provided in lesson**

### Class vs Functional
A brief explanation of when to use which and the pain points associated with each.
- Main Takeaways:
	- At inception it the running rule was to use `Class components` when you wanted to utilize `state` and `Function components` when you just wanted to render data via `props` and or `staticly`
	- Yet with the introduction  of `React Hooks` that all went out the window
		- Facebook's official recommendation is to use `functional` components whenever possible
			- Although many Developers and Engineer debate this point

### Build Two Components - **You Do**
Have students create a `functional` and `class` component on their own.
**Prompt provided in the lesson**

## Props and State
This is a brief overview of what is to be covered in the following sections: **Props** and **State**. 

### Props
- Main Takeaways:
	- `Props` is short for `properties`
	- `Props` are variables which store data
	- `Props` are `immutable`, meaning their value can not be changed
	- `Props` are passed into a component by its `parent` component

### Rendering Props - I Do
Build a `Functional` and `Class` component which both render `props`. 

### State
- Main Takeaways:
	- `State` is an JavaScrip object which is defined in the constructor of a `Class component`
	- `State`'s purpose is to hold data for a component
	- You are able to define variables with in `state` which can be accessed and rendered with in the component
	- `State` can also be pass the components's children components in the form a `Prop`

### Rendering State - I Do
Build a `Class` component that renders `state`. 

### Passing State and Rendering State - I Do
Utilize the `Class` component you just built and:
1. Replace the `JSX` you wrote with the `Functional` component you created earlier
2. Pass the `State` of the class component into the `Functional` component as `props`
3. Rework the `Functional` components `render` method so that the `JSX` is utilizing the `props` that were passed into the component 

### How do you conceptualize props and state - **Turn and Discuss**
Have student turn to their neighbor and discuss the following amongst themselves for 10 mins:
    - How they conceptualize props and state
    - What is the difference between prompts and state
**Provide a few more here**
Once 10 mins have lapsed call on one group for each prompt and have them explain what they discussed in regards to it.

## Check for Understanding
This section is meant to provide multiple assessments that instructors can utilize to test and quantify student understand of the lesson.

Assessment Questions:
- Is React a `library` or a `framework`
- Have each student in their own words define the following vocabulary words:
    - `Framework`
    - `library`
    - `Virtual DOM`
    - `JSX`
    - `Components`
    - `Functional Components`
    - `Class Components`
    - `Props`
    - `State`

## Further Reading
- Be giving to students as further reading to help solidify lesson concepts and or allow advance student more material to learn from 

# Instructor Prep Section
This section provides instructors extra details on the break down of this lesson.

# Delivery Tips:

* Think about how long you're talking
* Move quicker sooner, slower later
* Cold Call more often
* Revisit LOs
* Defer questions when appropriate

## Legend:
- I Do - Instructor-led demos
    - Students should `not` code along
- We Do - Instructor-led demos
    - Students should code along
- You Do - Test for understanding
    - Students should complete on their own
    - They can ask for instructor assistance
- Cold Call - Instructor calls on a random student(s) to answer prompt(s)
- Turn and Discuss - Student-led dialogue
    - Have students turn to their neighbor(s) and discuss the provided prompts
    - If time permits:
        - Once time allotted has lapsed the instructor should call on each group and have a representative talk about what their group discussed
- Breakout Groups - Break students into small groups to work through provided prompts
    - Typically 10-15 min time blocks

## Prep Resources
This section is meant to provide instructor helpful links that will assist them in preparing to teach this lesson. It should contain any resources that Curriculum Engineers used to write the lesson.

# Lesson Plan - Review Notes
This section is meant to collect instructor feedback on the lesson and lesson plan. **Could perhaps provide a link to a google form which asked the below questions**
Survey Questions:
1. Are the learning objectives present and complete?
2. What is the ratio of talking vs. doing? (60/40, TT/ST-wg vs ST-sg / individual)
3. What is the level of engagement?
4. Are exercise plans present?
5. Any pitfalls with the exercises?       