# IIFE (Immediately Invoked Function Expression)

```javascript

// example.js

(function iife(){

  // code in here
  var x = 5;
  x += 2;
  console.debug(x);

})();

```

First thing you see is here a **named** function wrapped in some braces. This is a named function because when deugging you will see a better stack trace that says something like ```iiffe() line 8``` instead of ```anonymous function line 8```. It just makes debugging easier.

The other thing that this function wrapped in braces does is that it hides the functions scope and does not polute the global name space. Which is key to the entire purpose of doing an iife in the first place. The purpose of the iife in general is to **hide code inside of it from the global namespace**. This prevents namespace collisions in libraries and also makes things cleaner in general because writing code in a global space is bad practice generally.

**tl;dr** The iife prevents poluting the global namespace. So the x variable is not in global and only exists within the iife function which is not exposed. 
