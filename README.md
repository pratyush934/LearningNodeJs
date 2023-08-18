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
