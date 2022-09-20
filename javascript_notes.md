# Notes

[Mozilla Docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript)

## variable assignment

var varName - old style
let varName - variable declaration
const varName - constant declaration

## Function declaration

[functions doc](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions)

```
funct myFunct() {}
const myFunct = () => {}
const myFunct = only_one_var => {}
const myFunct = (var1, var2) => {}
const multiply = (number) => number * 2;
const multiply = number => number * 2;
```

## export / import

```
export default person
import person from './person.js'
import prs from './person.js'

export person
import {person} from './person.js'
import {person as smith} from './person.js'
import * as people from './person.js'
```

## Classes

[Classes Doc](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

```
class Person extends Human {
    name = 'Andy'    // properties
    call = () => {}  // method
    constructor() {} // method that will get called when instantiating a class
}


```

usage

```
  const myPerson = new Person()
```

add `super()` to `constructor()` to child classes to call parent constructor.

`this` references class instance inside class

## Spread & Rest Operator

operator: `...`

spread: split up array elements or object properties

```
// create new array with values from old as well as `1` and `2`
const newArray = [...oldArray,1,2]
// create new object with elements from old as well as `newProp`
const newObject = {...oldObject,newProp:5}
```

rest: merge list of functionality arguements into an array

```
function sortArgs(...args) {
    return args.sort()
}

const filter = (...args) => {
    return args.filter(el => el === 1);
}
```

## Destructuring

Pulling elements out of arrays or objects and store in new object:

```
//Array
[a, ,b] = ['Hello','Max', 'Bob']
console.log(a) // Hello
console.log(b) // Bob

//Object
{name} = ({name: 'bob', age: 20})
console.log(name) // bob
```

## Primatives and Refrences

primatives are copied when assigned to new variable
| primatives |
| ---------- |
| number |
| string |
| boolean |

references are pointers to objects, assigning to new variable clones pointer not object
| reference types |
| ---------- |
| objects |
| arrays |

```
// copy primative
const number = 1;
cosnt num2 = number;
number = 2;
console.log(num2); // 1

// copy pointer to reference
const person = { name: 'Max'};
const secondPerson = person;
person.name = 'Manu';
console.log(secondPerson.name); // Manu

// to copy object use spread operator
const person = { name: 'Max'};
const secondPerson = {...person};
person.name = 'Manu';
console.log(secondPerson.name); // Max
```

## Array Functions

[Array documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)

| Function | description                                                                                                           |
| -------- | --------------------------------------------------------------------------------------------------------------------- |
| filter   | [filter documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter) |
| map      | [map documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)       |
| sort     | [sort documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)     |

```
const numbers = [1,2,3]
const doubleNumArray = numbers.map((num) => {return num * 2});

console.log(numbers); // [1,2,3]
console.log(doubleNumArray); // [2,4,6]
```

## syntax

| operator | description             |
| -------- | ----------------------- |
| `===`    | type and value equality |

```

```
