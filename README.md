# React-Schwarzmuller

## JavaScript

### Export-Import Modules

person.js
```
const person = {
  name: 'Maz'
}
```

import into app.js

```
import person from './person.js'
```

### Classes

In ES6, use constructor() to initialize class in ES6. Must be "super()" keyword if you extend the class. 

```
class Human {
  constructor() {
    this.gender = 'male';
  }

  printGender() {
    console.log(this.gender)
  }
}

class Person extends Human {
  constructor() {
    super();
    this.name = 'Max';
  }

  printMyName() {
    console.log(this.name);
  }
}

const person = new Person();

person.printMyName();
```


### Classes, Properties, and Methods

Constructor function and super keyword no longer needed. 


```
class Human {
  gender = 'male';
  
  printGender = () => {
    console.log(this.gender)
  }
}

class Person extends Human {

    name = 'Max';

  printMyName = () => {
    console.log(this.name);
  }
}

const person = new Person();

person.printMyName();
```

### Spread Operator

```
const numbers = [1,2,3];

const newNumbers = [...numbers,4];

console.log(newNumbers);
```

### Rest Operator

