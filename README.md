# js-fundamentals-and-oop
Resource for various JavaScript fundamentals, concepts, Object-Oriented JavaScript & other stufffff

## `null` and `undefined`
* `undefined` means a variable has been declared but has not yet been assigned a value
* `null` is an assignment value: it can be assigned to a variable as a representation of no value
* Also, `undefined` and `null` are two distinct types: `undefined` is a type itself, while `null` is an object.

e.g. looking up a property on an object which doesn't yet exist, or has not been assigned, will return `undefined`

`null !== undefined`
but...
`null == undefined`

* With default parameters, `undefined` will use the default -- while `null` does not.
* Both are two of JavaScript's *falsy* values, & both are *primitive* values.

## Closures
A closure is simply a **function inside another function**.
* ...when you want to extend behaviour (variables, methods, arrays) from an outer function to an inner function
* We can also access the context inside the outer function from the inner function -- but not the other way around

## Object-context; `this`

## Callbacks
A callback is a function that executes after another function has executed.
...it's a way to make asynchronous operations more synchronous

* Waits for an event to execute
* Provides synchronous capabilities
* Practical way to chain functionalities
* Provides code structure and control

**Callback hell**: *recursive* structure of callbacks

## Recursion

## Scope
Two types of 'scope' in JavaScript: **global** and **local**

Outermost-scope is global; when we declare a function, it creates a new instance of local-scope.
From inside that function block: we can reach outward to grab variables -- but we can't reach inward from global scope.

* Separates logic
* Narrows focus; improves code-quality
* Improves readability

## `call()`, `apply()`, and `bind()`

## Prototypal-inheritance

## The DOM

## The internetttttt 

## Cookies, session, and localstorage

## Currying

## MVC, & design-patterns

## IIFE

## Event-loop / the 'stack'

## Async / Await
Provides a way to maintain asynchronous-processing in a more synchronous fashion
* in that sense, have more control over the behaviour of your program

Most relevant: performing a REST API request -- you want the data to load before pushing it to the view. We use `await` to tell it to resolve fully before continuining

## Promises

## `fetch` API

## RESTful APIs
