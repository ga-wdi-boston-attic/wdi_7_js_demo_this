![General Assembly Logo](http://i.imgur.com/ke8USTq.png)

# What is `this`? 

![What is this?](http://i.giphy.com/bYGMDZP58u5bi.gif)

## Objectives

By the end of this, students should be able to:

- Recall whether or not `this` is determined at declaration.
- Explain what `this` points to in each calling context.
- Read and follow the execution context of code that uses different `this` idioms.

## `this` Is A Referent

> We use this similar to the way we use pronouns in natural languages like English and French. We write: “John is running fast because he is trying to catch the train.” Note the use of the pronoun “he.” We could have written this: “John is running fast because John is trying to catch the train.” We don’t reuse “John” in this manner, for if we do, our family, friends, and colleagues would abandon us. Yes, they would. In a similar aesthetic manner, we use the this keyword as a shortcut, a referent to refer to an object.
>
> Source: [Understanding Javascript 'this' pointer.](http://javascriptissexy.com/understand-javascripts-this-with-clarity-and-master-it/)

## `this` Changes by Call Context


## Summary

> 1. Is the function called with `new` (**new binding**)? If so, `this` is the newly constructed object.
>     `var bar = new foo()`
> 2. Is the function called with `call` or `apply` (**explicit binding**), even hidden inside a `bind` *hard binding*? If so, `this` is the explicitly specified object.
>     `var bar = foo.call( obj2 )`
> 3. Is the function called with a context (**implicit binding**), otherwise known as an owning or containing object? If so, `this` is *that* context object.
>     `var bar = obj1.foo()`
> 4. Otherwise, default the `this` (**default binding**). If in `strict mode`, pick `undefined`, otherwise pick the `global` object.
>     `var bar = foo()`
>
> Source: [You-Dont-Know-JS/ch2.md](https://github.com/getify/You-Dont-Know-JS/blob/58dbf4f867be0d9c51dfc341765e4e4211608aa1/this%20&%20object%20prototypes/ch2.md)

## Lab (Pair)

Pair with a partner and review each of the following examples in order. Your goal in this assignment is to read and understand the code examples presented. Take time to contemplate the execution flow, and note any questions you have for discussion.

For each example, you will edit `app/this.html` to include the appropriate script from `app/js`.  Review the script for instructions before you refresh your browser window. Many of this scripts use the special `debugger` keyword to stop JS execution and open your console. Use this opportunity to inspect your environment (perhaps by looking at `this`?) and then [continue](https://developer.chrome.com/devtools/docs/javascript-debugging).

- `object_literal.js` - 'this' in an object literal.
- `global_function.js` - 'this' in a global function.
- `event_handler_broken.js` - Broken button event handler.  
- `event_handler_fixed.js` - Fixed button event handler.
- `inner_function_bad.js` - Broken inner function.  
- `inner_function_fixed.js` - Fixed inner function.  
- `reassign_method_bad.js` - Changing the runtime context of a method to the global object.
- `reassign_method_fixed.js` - Changing the runtime context of a method with the javscript _bind_ function.

## Additional Resources

- [Understand JavaScript’s “this” With Clarity, and Master It | JavaScript is Sexy](http://javascriptissexy.com/understand-javascripts-this-with-clarity-and-master-it/)
- [You-Dont-Know-JS/README.md at master · getify/You-Dont-Know-JS](https://github.com/getify/You-Dont-Know-JS/blob/master/this%20&%20object%20prototypes/README.md#you-dont-know-js-this--object-prototypes)
