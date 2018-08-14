## Trace-blocking-errors

Trace Blocking errors in a code snippet (using the try-catch method). Object properties and assignment operators.

### Index
* [Learning Objective](#learning-objective)
* [Study Snippet](#study-snippet)
* [Practice Points](#practice-points)
* [Helpful Links](#helpful-links)
___

## Learning Objective

Language Features:
* '+=' assignment operator with objects and properties 
* '.' member access operator (dot notation)


[TOP](#index)

___
 
## Study Snippet

```js
let obj = {a: 0, b: 1, c: 2}, x = "c"; 
(((obj.a += 2).b += 1)[x] += 0);

//Breakdown
obj.a += 2;
//Reached an error
try {
  2.b += 1;
} catch (err) {
  console.log(err);
  obj.b += 1;
};
//Reached another error
try {
  2[x] += 0;
} catch (err) {
  console.log(err);
  obj[x] += 0;
};

```

[PyTut](https://goo.gl/icM8MS)

[TOP](#index)

___

## Practice Points:

[TOP](#index)

## Helpful Links

* +=: [w3schools](https://www.w3schools.com/js/js_assignment.asp)
* . : [MDN] (https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Property_Accessors#Dot_notation)

[TOP](#index)
