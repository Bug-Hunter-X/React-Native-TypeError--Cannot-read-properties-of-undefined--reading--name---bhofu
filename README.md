# React Native TypeError: Cannot read properties of undefined (reading 'name')

This repository demonstrates a common error in React Native applications: `TypeError: Cannot read properties of undefined (reading 'name')`. This error arises when attempting to access a property of an object before the object itself is properly initialized or defined.

## Bug Description:

The error occurs when trying to access the `name` property of a `user` object within the component's render method, even when using optional chaining (`?.`) or nullish coalescing (`??`), due to the `user` object not being set correctly initially within the component's state.  This usually occurs when asynchronous operations that set the user object haven't completed by the time the component tries to render.