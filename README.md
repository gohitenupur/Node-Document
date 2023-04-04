# Node-Document
Learn Node with basics

* 2009 -Node.js Created by Ryan Doll
* 2011 -npm created which allowed for the sharing of the open source libraries
* The node.js was formed in 2015

<h2>Inspecting the global object </h2>
-> global object is similar like the window or document object in js 
-> In Node.js, the global object is an object that contains properties and methods that are available globally throughout the application. 
   It is similar to the window     object in a browser environment.
-> The global object in Node.js includes several built-in properties and methods, such as:

--console: Provides methods for logging information to the console.
--process: Provides information about the current Node.js process, and methods for interacting with it.
--Buffer: Provides methods for working with binary data.
--setImmediate() and clearImmediate(): Provides a way to execute a function asynchronously, similar to setTimeout() and clearTimeout().
--setTimeout() and clearTimeout(): Provides a way to execute a function after a specified amount of time, and to cancel the execution if necessary.

** Note -Node.js uses chrome V8 interpreter

Ex - console.log(__dirname)
     console.log(__filename)
     
