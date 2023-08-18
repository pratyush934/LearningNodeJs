# LearningNodeJs

# NODE.JS

JavaScript Runtime Environment
It is used for server side programming

Node.js is not a language, library or framework.

# Node REPL

REPL -> Read , Evaluate , Print, Loop

# Process

1. process :
   This object provides information about, and control over, the current Node.js process.
2. process.argv : returns an array containing the command-line arguments passed when the Node.js process was launched
   let args = process.argv;

for (let i = 2; i < args.length; i++) {
console.log("Hello & Welcome to ", args[i]);
}

# Module Exports

1. requiring files
   require() -> a built-in function to include external modules that exist in seperate files.
   
   const someValue = require('./math');
   console.log(someValue);

   module.exports -> a special object
   --> module.exports = "hello";


# NPM (Node Package Manager) :
npm is the standard package manager for Node.js
1. Library of packages
2. Very Useful for people

TO USE THIS PACKAGES.
npm install folderName (Folder name must be within directory)

1. node_modules : THe node modules folder contains every installed dependency for your project.
2. package-lock.json : It records the exact version of every 
installed dependency, including its sub-dependencies and their versions.
It contains descriptive and functional metadata about a project such as a name, version, and dependencies.

# LOCAL v/s GLOBAL
npm install -g <package-name>
npm link <package-name>

# REQUIRE V/S IMPORT
import {sum} from "./maths.js"

We can't selectively load only the pieces we need with require but with import, we can selectively load only the piece we need, which can save memory.

Loading is synchronous for 'require' but can be asynchronous for 'import'.

# DONO ME SE KOI EK HI HAI

export const sum = (a, b) => a + b;
export const mul = (a, b) => a * b;
export const g = 9.8;
export const g = 3.14;

ALAG FILE ME
import {sum, PI} form "./math.js"