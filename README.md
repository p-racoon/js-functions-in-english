# js-functions-in-english
In this repo, I intend to describe/express commonly used Built-in JS Object's properties and methods in English.<br/>
***i.e How a given function can be read in English.*** <br/>
>e.g. `[1,2,3].pop()` method can be read as: `"pop/remove from the last value from the original array and return the popped/removed value."`<br/>

## JS Array
### 1. concat()
**[Array.prototype.concat()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/concat)**

`const newArray = array.concat([value1[, value2[, ...[, valueN]]]])`
>shallow copy all the values of the `old_array` into a new array, along with all the elements of the array/values provided as parameters into a new array.

*If no parameters are provided shallow copy of `old_array` is returned.*

### 2. copyWithin()
**[Array.prototype.copyWithin()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/copyWithin)**

`const modifiedArray = array.copyWithin(target[, start[, end]])`
>*shallow copy* all the values from within the array `arr` from *index* `start` to *position* `end` and *paste* it to the same array starting from `start` *index*.

*If `end` parameter is skipped the values are copied from `start` till end of the array.*

### entries()
**[Array.prototype.entries()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/entries)**

```
  const arrayIterator = array.entries()
  for (const [index, element] of arrayIterator)
    console.log(index, element);
```
>return an *iterator object* to iterate over the `array`

### every()
**[Array.prototype.every()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/copyWithin)**

`const booleanResult = array.every(callback(element[, index[, array]])[, thisArg])`
>iterate over the `array` passing in each `element`, `index`, `array` to the `callback` function, and checking if all the return values from `callback` are *truthy* or not, if any one of them is *falsy* every stops its execution, and returns false. If all are true it returns `true`. Can pass an optional `thisArg` so that callbacks can be called as `thisArg.callback(element[, index[, array]])` internally.

*This method returns `true` for any condition put on an empty array.*

### fill()
**[Array.prototype.fill()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/fill)**

`const modifiedArray = array.fill(value[, start[, end]])`
>starting from `start` index till the `end` position of the array, fill with the given `value`.

*If only `value` is provided it fills the whole array with `value`.*

### filter()
**[Array.prototype.filter()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/filter)**

`const newArray = array.filter(callback(element[, index[, array]])[, thisArg])`
>iterate over the `array` passing in each `element`, `index`, `array` to the `callback` function, and checking if all the return values from `callback` are *truthy* or *falsy*, if *truthy* that `element` is pushed to the *outputArray*, otherwise skipped from beingPushed. At the end of iteration the *outputArray* is returned.

*If no elements pass the test(i.e. for none of the `element` `callback` returns a truthy value), an empty array `[]` will be returned.*

### find()

### findIndex()

### forEach()

### from()

### includes()

### indexOf()

### isArray()

### join()

### keys()

### length

### lastIndexOf()

### map()

### pop()

### prototype

### push()

### reduce()

### reduceRight()

### reverse()

### shift()

### slice()

### sum()

### sort()

### splice()

### toString()

### unshift()

### valueOf()
