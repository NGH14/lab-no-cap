# [Variable scope](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Grammar_and_types#variable_scope)

>__The default scope for all code running in script mode__. When you declare a variable outside of any function, it is called a global variable, because it is available to any other code in the current document. When you declare a variable within a function, it is called a local variable, because it is available only within that function.

## [Global scope](https://developer.mozilla.org/en-US/docs/Glossary/Global_scope)

>Global scope means variables are accessible from anywhere in the code

__Note__:In a browser environment like Firefox, Google Chrome, ect. Global variables become properties of the `window` object.

List [JS global object](https://developer.mozilla.org/en-US/docs/Glossary/Global_object):

```js
console.log(globalThis === globalThis.globalThis); // true (everywhere)
console.log(window === window.window); // true (in a browser)
console.log(self === self.self); // true (in a browser or a Web Worker)
console.log(frames === frames.frames); // true (in a browser)
console.log(global === global.global); // true (in Node.js)
```

![global Variable](image.png)

## [Function scope](https://www.greatfrontend.com/questions/quiz/explain-the-difference-between-global-scope-function-scope-and-block-scopee)

>Every function in JavaScript creates its own scope, known as function scope. Variables declared within a function are accessible only within that function.



