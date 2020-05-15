### OOP in JavaScript

## 4 pillars OOP

1. Encapsulation
2. Abstraction
3. Polimorphism
4. Inheritance

## Procedural Programming

Function and data. Big project. Hell of functions => spagetti-code.

## OOP

Car:
- data - color, weigth, name
- methods - start(), stop()

Ex. localStorage - length is data and many methods.

### 1. Encapsulation 

Benefits: group code -> reduce complexity + increse reusability;

> "The best function are those with no parameters" (Uncle Bob - Robert Martin)



### 2. Abstraction

Benefits: reduce complexity + isolate code;

DVD player, many buttons, but we dont care how their works.

В объекте часть методов смотрят наружу, кт используют пользователи, а часть скрыта. Ту часть можно менять не боясь за публичные методы..

### 3. Inheritance

Benefits: Eliminate redundunt code

Для того чтобы уменьшуть дублирование кода. Eliminate redundunt code.

Например, 3 элемента, - TextBox, Select, CheckBox, у них общие:
- hidden, innerHTML
- click(), focus()

### 4. Poly (many) morphism (forms)

Benefits: Refactor ugly switch/case statement

```js
// procedural way
switch() {}
'select': renderSelect();
'textbox': renderTextBox();
...
}

// oop
element.render();

```

## 2. Setting Up Envirement

- VSCode: live server extensin
- `!`
- `open with live server`

## 3. Objects
17:15

```js
const circle1 = {
  radius: 1,
  location: {
    x: 1,
    y: 1
  },
  draw: function() {}
}

const circle2 = {
  radius: 1,
  location: {
    x: 3,
    y: 3
  },
  draw: function() {}
}

// not good: dublicate methods
```

**Refactor. Two Way**

**1. Meet Factory Function**

Many dev like this.

```js
function createCircle(radius) {
  return {
    radius, // ES6 feat, instead `raduis: radius`
    draw: function() {}
  }
}

const circle = createCircle(1)
circle.draw()
```

**2. Constructor Function**

C# like this way

`new` operator
- new make {}
- automatic return

```js
function Circle() {
  console.log(this)
}
const c1 = Circle(); // Window
const c2 =new Circle(); // Circle
```

```js
  function Circle(radius) {
    this.radius = radius;
    this.draw = function() {
      console.log('draw')
    }
  }
  const c =new Circle();
```
