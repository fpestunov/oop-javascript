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

# 2. Setting Up Envirement

- VSCode: live server extensin
- `!`
- `open with live server`

