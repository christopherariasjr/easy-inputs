## easy-inputs v1.0.0
---
__Easy__ terminal inputs for an __Easy__ time.

### Installation
---
```
npm install easy-inputs

yarn add easy-inputs
```

### How to use
---

```
const ez = require('easy-inputs');

//Text prompt
//Text prompt returns a "String" data type.

var name = ez.text('What is your name?: );

//Number prompt
//Number prompt returns a Number data type

var name = ez.number('What is your age?: );

//Question propmt allows you to get a closed-ended question from the user
//The array needs to be two objects and have a name and value element
//An optional "default" element is applicable to allow the user to continue with a default answer

var dog = ez.question('Are you a dog? [y/N]: ', [
    {
        name: 'y',
        value: true,
    },
    {
        default: true,
        name: 'n',
        value: false,
    }
])
```