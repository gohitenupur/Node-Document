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
     <h4>In Node.js, the path module provides utilities for working with file and directory paths. This module provides a way to manipulate file paths regardless of the underlying operating system.</h4>
     

<p>Some of the methods provided by the path module include:</p>
<ul>
<li>path.join([...paths]): Joins all given path segments together using the platform-specific separator as a delimiter, then normalizes the resulting path.</li>
<li>path.normalize(path): Normalizes a path, resolving '..' and '.' segments.</li>
<li>path.resolve([...paths]): Resolves a sequence of paths or path segments into an absolute path.</li>
<li>path.dirname(path): Returns the directory name of a path.</li>
<li>path.basename(path[, ext]): Returns the last portion of a path, optionally removing a file extension.</li>
<li>path.extname(path): Returns the file extension of a path.</li>
</ul>

<P>
const path = require('path'); // Import the path module
const myPath = path.join('/Users/john', 'Documents', 'file.txt'); // Join the path segments together
console.log(myPath); // Output the resulting path
</p>

<h2>Process</h2>
<h4>In Node.js, the process object is a global object that provides information about and control over the current Node.js process. The process object emits a variety of events that you can use to respond to various state changes in the Node.js process.</h4>

<p>Some of the most commonly used events emitted by the process object include:</p>
<ul>
<li>'exit': Emitted when the Node.js process is about to exit.</li>
<li>'uncaughtException': Emitted when an unhandled exception occurs in the Node.js process.</li>
<li>'SIGINT': Emitted when the Node.js process receives a SIGINT signal (e.g., when the user presses Ctrl+C).</li>
<li>'SIGTERM': Emitted when the Node.js process receives a SIGTERM signal.</li>

</ul>

<h3>In Node.js, the process object provides access to the standard input (stdin) and standard output (stdout) streams of the current process.</h3>

process.stdin.on('data', (data) => {
  console.log(`Received data: ${data}`);
});

<h3>The stdout stream is a writable stream that represents output to the user or to a file. You can write data to stdout using the process.stdout.write() method:</h3>

process.stdout.write('Hello, world!\n');


