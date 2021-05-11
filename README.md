# Functional Programming - React - JS

## 1 Javascript Equality
```javascript
var a = [1,2,3]
var b = [1,2,3]
var c = "1,2,3"

console.log(a == b)
console.log(b == c)
console.log(a == c)
```
Shows the output of console.log

## 2 Hoisting - Immediately Invoked Function Expressions
```javascript
var a = 42

(function IIFE(){
var a = 10;
     console.log( a )
})()

console.log(a)
```
Shows the output of console.log

## 3 Closure - Arrow Function - Anonymous Function
```javascript
function makeAdder(x) {
    function add(y) {
          return y + x
    }
  return add
}
```

Rewrite the statement using the arrow function

## 4 Lexical Scope 
```javascript
(function foo(a) {
     var b = a * 2
     function bar(c) {
         console.log( a, b, c )
     }
  bar(b * 3)
})(4)
```

Shows the output of console.log

## 5 Dynamic Scope 
```javascript
function foo() {
    console.log( a )
}
function bar() {
    var a = 3
    foo()
}
var a = 2
bar()
```

Shows the output of console.log

## Callstack
```javascript
setTimeout(() => {
  console.log('foo')
}, 0)
console.log('bar')
```

Shows the output of console.log

## 7 Immutable React State

What happens when modify this.state directly

## 8 Performace render

What is the Virtual DOM?



# Object Oriented Programming - Kotlin - Swift

## 1 Companion Object - Singleton

How to initialize a static variable in kotlin?

## 2 Rerform lazy-initialization

What is lazy in Kotlin/Swift ?

## 3 Define properties and methods 

What is different of Data Class (Kotlin)/ Struct (Swift) and Classes


# Algorithm

## 1 

Write pseudocode to simulate the elevator's processing algorithm.
```javascript
enum Direction {
  UP, DOWN
}

enum ElevatorState {
  UP, DOWN, OPEN_DOOR
}
```
input: { numberOfFloors: number, command: Direction }
output: interval(1000) -> { numberOfFloors: number, state: ElevatorState }
