# Introduction to Redux

Redux is a predictable state container for JavaScript apps. It helps you write applications that behave consistently, run in different environments (client, server, and native), and are easy to test.

## 01) Create a Redux Store

In Redux, there is a single state object that's responsible for the entire state of your application. This means if you had a React app with ten components, and each component had its own local state, the entire state of your app would be defined by a single state object housed in the Redux store. This is the first important principle to understand when learning Redux: the Redux store is the single source of truth when it comes to application state.

```javascript
const reducer = (state = 5) => {
  return state;
}

const store = Redux.createStore(reducer);
```

## 02) Get State from the Redux Store
The Redux store object provides several methods that allow you to interact with it. For example, you can retrieve the current state held in the Redux store object with the **getState()** method.

```javascript
const currentState = store.getState();
```

## 03) Define a Redux ActionPassed
Since Redux is a state management framework, updating state is one of its core tasks. In Redux, all state updates are triggered by dispatching actions. An action is simply a JavaScript object that contains information about an action event that has occurred. 

```javascript
// action simply is a JS object
const actions = {
  type: 'LOGIN'
}
```

```javascript

```