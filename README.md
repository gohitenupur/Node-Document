# Node-Document
Learn Node with basics

* <P>2009 -Node.js Created by Ryan Doll</p>
* <P>2011 -npm created which allowed for the sharing of the open source libraries</p>
* <P>The node.js was formed in 2015</p>

<h2>Inspecting the global object </h2>
-> <P>global object is similar like the window or document object in js </p>
-> <P> In Node.js, the global object is an object that contains properties and methods that are available globally throughout the application. 
   It is similar to the window object in a browser environment.</p>
-><P> The global object in Node.js includes several built-in properties and methods, such as:</p>


<P>--console: Provides methods for logging information to the console.</p>
<P>--process: Provides information about the current Node.js process, and methods for interacting with it.</p>
<P>--Buffer: Provides methods for working with binary data.</p>
<P>--setImmediate() and clearImmediate(): Provides a way to execute a function asynchronously, similar to setTimeout() and clearTimeout().</p>
<P>--setTimeout() and clearTimeout(): Provides a way to execute a function after a specified amount of time, and to cancel the execution if necessary.</p>

***** Note -Node.js uses chrome V8 interpreter *****

Ex - console.log(__dirname)
     console.log(__filename)
     
   <h2>Path Module</h2>
     <p>In Node.js, the path module provides utilities for working with file and directory paths. This module provides a way to manipulate file paths regardless of the underlying operating system.</p>
     

<p>Some of the methods provided by the path module include:</p>

<p> --path.join([...paths]): Joins all given path segments together using the platform-specific separator as a delimiter, then normalizes the resulting path.</p>
<p> --path.normalize(path): Normalizes a path, resolving '..' and '.' segments.</p>
<p> --path.resolve([...paths]): Resolves a sequence of paths or path segments into an absolute path.</p>
<p> --path.dirname(path): Returns the directory name of a path.</p>
<p> --path.basename(path[, ext]): Returns the last portion of a path, optionally removing a file extension.</p>
<p> --path.extname(path): Returns the file extension of a path.</p>

<P>
const path = require('path'); // Import the path module
const myPath = path.join('/Users/john', 'Documents', 'file.txt'); // Join the path segments together
console.log(myPath); // Output the resulting path
</p>

