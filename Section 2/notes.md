## Javascript engine?
#### Translate javascript code into computer 0 1

---

## Who built it?
#### Brandon Eich

---

## Whats ECMAscript?
#### Standard format of JS & engines (some kind of law)

---

## Interpreter? (JS)
#### Translate & read the codes line by line

---

## JS compilers
```
Have you heard of Babel or TypeScript? They are heavily used in the Javascript ecosystem and you should now have a good idea of what they are:

Babel is a Javascript compiler that takes your modern JS code and returns  browser compatible JS (older JS code).
Typescript is a superset of Javascript that compiles down to Javascript.

Both of these do exactly what compilers do: Take one language and convert into a different one!
```

---

## JIT compiler
#### Combine both interpreted and compiler to translate the codes

---

## Is javascript an interpreted language?
#### initially yes, but now we have some compilers for it !

---

## Problematic things in JS

- eval()
- arguments
- for in
- with
- delete
- hidden classes
- inline caching
 
[Wiki link](https://github.com/petkaantonov/bluebird/wiki/Optimization-killers)

---

## inline caching
#### Define data as variable so compiler will cache it

```js
function findUser(user) {
    return `User name is ${user.name}`
}

const userData = {
    name: 'Sina'
}

// after some while the userData will
// cache in compiler and prevent code calculation
findUser(userData)

```

---

## Call stack & memory Heap
#### Memory Heap

```js
const number = 100; // allocate memory for number
const string = "Sina"; // allocate memory for a string
const human = {
    first: 'Sina',
    last: 'Farhadi'
}; // allocate memory for object .... and it's values

```

#### Call stack is managing tasks and doing jobs with top in last out method

---

## Stack Overflow
#### When call stack become to much large : D

---

## Is JavaScript garbage collected language?
#### Yes, it is

---

## What it mean " Garbage Collected " ?
#### Clean unused allocated memory automatically

---

## How JavaScript do it?
#### With mark & sweep way

---

## Common memory leaks in JS

- Global variables
- Event listeners
- Set Intervals

---

## Javascript is Single Threaded language!
#### It not doing multiple things at same time :blush

---

## WebAPI
#### accessible in JS by "window" and allow to do asynchronous tasks in JS
#### Actually apis provided by browsers

---

## Window api pass the tasks to event loop
#### when calling web apis, the call stack push task to event loop and get the response when it's ready