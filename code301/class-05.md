# React Doc

![pic](https://th.bing.com/th/id/R.030029ff86ba2ead239db9736937801d?rik=vic78G5DKw83Gw&pid=ImgRaw&r=0)

## Step 1: Break The UI Into A Component Hierarchy

The first thing you’ll want to do is to draw boxes around every component (and subcomponent) in the mock and give them all names. If you’re working with a designer, they may have already done this, so go talk to them! Their Photoshop layer names may end up being the names of your React components!

## Step 2: Build A Static Version in React

To build a static version of your app that renders your data model, you’ll want to build components that reuse other components and pass data using props. props are a way of passing data from parent to child. If you’re familiar with the concept of state, don’t use state at all to build this static version. State is reserved only for interactivity, that is, data that changes over time. Since this is a static version of the app, you don’t need it.

## Step 3: Identify The Minimal (but complete) Representation Of UI State

To make your UI interactive, you need to be able to trigger changes to your underlying data model. React achieves this with state.

## Step 4: Identify Where Your State Should Live

For each piece of state in your application:

+ Identify every component that renders something based on that state.
+ Find a common owner component (a single component above all the components that need the state in the hierarchy).
+ Either the common owner or another component higher up in the hierarchy should own the state.
+ If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.

## Step 5: Add Inverse Data Flow

React makes this data flow explicit to help you understand how your program works, but it does require a little more typing than traditional two-way data binding.