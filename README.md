# Object-oriented Programming in JavaScript

Object-oriented Programming in JavaScript course by Mosh Hamedani

<p align="center">
  <a href="https://www.udemy.com/course/javascript-object-oriented-programming" rel="noopener">
 <img src="https://img-b.udemycdn.com/course/240x135/1642074_7ef3.jpg" alt="Project logo"></a>
</p>

## Course Plan 👇

1. Getting Started
2. Objects
3. Prototypes
4. Prototypical Inheritance
5. ES6 Classes
6. ES6 Modules

## Getting Started

### What is OOP ?

-- Object-oriented programming is a programming <b>paradigm</b> centered around objects rather than functions.
-- OOP is not a programming language or tool!

### Four Pillar is OOP

1. **Encapsulation**: Bundling data and methods that operate on that data within objects, restricting direct access to some of the object's components.

```js
class Person {
  #name; // private field
  constructor(name) {
    this.#name = name;
  }
  getName() {
    return this.#name;
  }
}
const person = new Person("Alice");
console.log(person.getName()); // Alice
```

2. **Abstraction**: Hiding complex implementation details and showing only the necessary features of an object.

```js
class Car {
  startEngine() {
    // Complex logic hidden from user
    console.log("Engine started");
  }
}
const car = new Car();
car.startEngine(); // Engine started
```

3. **Inheritance**: Mechanism for creating new classes from existing ones, enabling code reuse and the creation of hierarchical relationships.

```js
class Animal {
  speak() {
    console.log("Animal speaks");
  }
}
class Dog extends Animal {
  speak() {
    console.log("Dog barks");
  }
}
const dog = new Dog();
dog.speak(); // Dog barks
```

4. **Polymorphism**: Ability of different objects to respond, each in its own way, to the same method or property.

```js
function makeSound(animal) {
  animal.speak();
}
const animals = [new Animal(), new Dog()];
animals.forEach(makeSound);
// Output:
// Animal speaks
// Dog barks
```

<a href="https://www.udemy.com/certificate/UC-257ffdc3-16c7-471f-b219-79d83a4404e8" rel="noopener">
<img src="https://udemy-certificate.s3.amazonaws.com/image/UC-257ffdc3-16c7-471f-b219-79d83a4404e8.jpg" alt="Project logo">
</a>
