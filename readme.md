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

## Class

- ES6

```js
class Araba {
    constructor(renk) {
        this.renk = renk;
        this.hız = 0;
    }

    hızlandır() {
        this.hız += 10;
    }
}
let araba = new Araba("siyah");
console.log(araba.renk); // "siyah"
console.log(araba.hız); // 0
araba.hızlandır();
console.log(araba.hız); // 10

```

- ES5

```js
function Araba(renk) {
    this.renk = renk;
    this.hız = 0;
}

Araba.prototype.hızlandır = function() {
    this.hız += 10;
};

let araba = new Araba("siyah");
console.log(araba.renk); // "siyah"
console.log(araba.hız); // 0
```