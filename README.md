## RxJS by Example:

1. https://codeburst.io/rxjs-by-example-part-1-ff7f1530071c
2. https://codeburst.io/rxjs-by-example-part-2-8c6eda15bd7f
3. https://codeburst.io/rxjs-by-example-part-3-7f37ffa8b9d6
4. https://codeburst.io/rxjs-by-example-part-4-939603ed3fac 
  * We end this series by writing the core functionality of Redux in three lines of RxJS code; A real testimony on RxJS. Wow!

Other references:

1. https://www.learnrxjs.io/learn-rxjs/concepts/rxjs-primer
2. https://www.youtube.com/watch?v=bn8qsi8jVew&t=1s
3. https://codeburst.io/why-redux-in-four-drawings-511b54788ec7

## Installation
```
yarn install #did not work. Problems with fsevents
```

**Switched to npm and node v18.0.0**

Instead of:

```
yarn run babel src -d dist
```

I did:

```
✗ npx babel src -d dist
```

## Hello World

```
➜  rxjs-patterns git:(master) ✗ node dist/hello-world.js 
Normal
1 + !!!
2 + !!!
3 + !!!
RxJS
1 + !!!
2 + !!!
3 + !!!
```

## Asynchronous

See `src/hello-world.js` for the code.

```
 ✗ node dist/asynchronous.js
Normal
RxJS
```

## Combining asynchronous operations

Given three asynchronous operations, we perform them back to back; logging their output to the console with the results (each pair of lines appearing one second after the previous pair).

```
➜  rxjs-patterns git:(master) ✗ node dist/combined.js 
Normal A
RxJS A
Normal B
RxJS B
Normal C
RxJS C
```

![](https://codeburst.io/rxjs-by-example-part-1-ff7f1530071c)

As we saw through the examples, an Observable is a collision between a Promise and an Iterator (Array). 