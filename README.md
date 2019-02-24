# getFirstIndexOf(value, array): number

Returns index of first instance of `value` found in `array`.  
`value` can be a primitive or array .  Returns -1 if `value` not found.


# getLastIndexOf(value, array): number

Returns index of last instance of `value` found in `array`.  
`value` can be a primitive or array.  Returns -1 if `value` not found.


# getIndexOfPrimitive(<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;primitive,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;array,<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;startingPosition? = 0<br>): number

Behaves like `Array.indexOf()`, except it does strict type-checking on `primitive`.  
Change `startingPosition` to get something other than the first index.  
`startingPosition` can also be negative to search from the end.  
Returns -1 if `primitive` not found.


# getIndexesOf(value, array): number[]

Returns all indexes of `value` in `array`.  
`value` can be a primitive or array. 


# getIndexesThatPass(testFunction, array): number[]

This returns all indexes of array items that pass the `testFunction`.  
`testFunction = function(currentValue, currentIndex?, theArray?): boolean`
```
Example:

let arr = ['a', 'boy', 'is', 'playing', 'in', 'the', 'street'];

let stringsLongerThanThree = getIndexesThatPass((value) => value.length > 3,  arr);
// stringsLongerThanThree is now [3, 6]
```

## Installation
`npm i  @writetome51/array-get-indexes`


## Loading
```
// if using TypeScript:
import {getFirstIndexOf, getLastIndexOf, getIndexOfPrimitive, getIndexesOf, getIndexesThatPass} 
    from '@writetome51/array-get-indexes'
    
// if using ES5 JavaScript:
var getFirstIndexOf = require('@writetome51/array-get-indexes').getFirstIndexOf;
var getLastIndexOf = require('@writetome51/array-get-indexes').getLastIndexOf;
var getIndexOfPrimitive = require('@writetome51/array-get-indexes').getIndexOfPrimitive;
var getIndexesOf = require('@writetome51/array-get-indexes').getIndexesOf;
var getIndexesThatPass = require('@writetome51/array-get-indexes').getIndexesThatPass;
```