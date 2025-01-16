# React Native: 'this' is undefined - Functional Component Error

This repository demonstrates a common error in React Native where the 'this' keyword is incorrectly used within a functional component. Functional components in React do not have their own 'this' binding.

## The Problem

The `bug.js` file shows how attempting to use 'this' inside a functional component results in a runtime error.  This often occurs when trying to bind event handlers or use lifecycle methods (though lifecycle methods aren't directly applicable to functional components).

## The Solution

The solution in `bugSolution.js` demonstrates how to solve this by using hooks or arrow functions to correctly handle the context and binding of event handlers.  Arrow functions lexically bind 'this', providing the correct context.