## Import - Exports

```js
const { tutorial } = require('tutorial.js');

var name = "Egemen"
var age = 19

tutorial(name, age)
```

```js
export const tutorial = (name, age) => {

  console.log("İsmi:"+ name +" Yaşı:"+ age);

};
```