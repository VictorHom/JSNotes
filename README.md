# Notes

What does 'use strict' do?
- throws error when you define a variable as global variable
- deleting undeletable properties will throw an error
- cannot set properties on primitive values
- in a function, this now refers to undefined instead of the global object

What does object.create do?
- it takes an object as the first arg and a second, optional arg is an obj that goes to Object.defineProperties
- it sets the new object's internal property to be the constructor function's external accessible prototype object.
- it returns the newly created object

What does new operator do?
- it creates a new object
- it sets the object's internal prototype to be constructor function's external, accessible prototype object.
- it executes the constructor, using the newly created object whenever this is mentioned. the newly constructed object is set as the this binding for that function call.
-  it returns the newly created object, unless you set the return to be something. Probably shouldn't set the return.


What is difference between new and Object.create?
- unlike the new operator, object.create does not execute a constructor function with newly created object, thereby giving it own properties.
