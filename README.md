<p align="center"><a href="https://typeis.github.io/" target="_blank"><img width="200"src="https://typeis.github.io/typeis.png"></a></p>

#typeis.js
##Typeis. it's the smart and simple javaScript type checker;


###Download

* [typeis.js](https://raw.githubusercontent.com/typeis/typeisjs/master/typeis.js) ([minified](https://raw.githubusercontent.com/typeis/typeisjs/master/dist/typeis.min.js))

###installation
```javascript
npm install typeis
bower install typeis
```
###usage
In Node.js:
```javascript
require('typeis');
```
In a browser:
```html
<script src="typeis.js"></script>
```
####examples
```javascript
var regexp = /test/gi
var arr = ['test'];
var now = new Date();
var obj = {};

console.log(regexp.typeis()); //RegExp;
console.log(regexp.typeis('regexp')); //true;
console.log(regexp.typeis('object')); //false;
console.log(arr.typeis()); //Array;
console.log(arr.typeis('array')); //true;
console.log(now.typeis()); //Date;
console.log(obj.typeis()); //Object;
```

####Real world Usage

```javascript 
function realWorld( options ){
    if(options.typeis('object')){
        //do something
    } else {
        //do another something
    }
}
```
