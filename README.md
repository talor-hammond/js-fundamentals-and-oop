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

## sessionStorage, localStorage, cookies
sessionStorage, localStorage and Cookies all are used to store data on the client side. Each one has its own storage and expiration limit.

**localStorage:**
* Web storage can be viewed simplistically as an improvement on cookies, providing much greater storage capacity. Available size is 5MB which considerably more space to work with than a typical 4KB cookie.
* The data is not sent back to the server for every HTTP request (HTML, images, JavaScript, CSS, etc) - reducing the amount of traffic between client and server.
* The data stored in localStorage persists until explicitly deleted. Changes made are saved and available for all current and future visits to the site.
**cookies:**
* We can set the expiration time for each cookie
* The 4K limit is for the entire cookie, including name, value, expiry date etc. To support most browsers, keep the name under 4000 bytes, and the overall cookie size under 4093 bytes.
* The data is sent back to the server for every HTTP request (HTML, images, JavaScript, CSS, etc) - increasing the amount of traffic between client and server.
**sessionStorage:**
* Similar to localStorage, but once the window is closed, the storage is deleted
* The data is available only inside the window / tab it was set

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
* Programming API / JavaScript Object Representation of our webpage
* Defines the logical structure of documents and the way a document is accessed and manipulated
    * Exposes methods like `.addEventListener()` on pieces of the webpage
    * Manipulate styles, animation, deletion, change values

## The internetttttt 

## Cookies, session, and localstorage

## Currying

## MVC, & design-patterns

## IIFE
'Immediately-invoked function expressions'
- Function is fired immediately after declaration

- Avoids 'polluting' code; code-clarity

## Event-loop / the 'stack'

## Async / Await
Provides a way to maintain asynchronous-processing in a more synchronous fashion
* in that sense, have more control over the behaviour of your program

Most relevant: performing a REST API request -- you want the data to load before pushing it to the view. We use `await` to tell it to resolve fully before continuining

## `fetch` API
Interface provided by the browser which lets us make XMLHttpRequests to other places on the web.
* Extremely tedious to do manually, so we can use a library like `superagent` to make our lives easier

## RESTful APIs
