# hans-obj-comparator
With this package it is available to compare Objects and Arrays

## Table of contents
* [Installing](#installing)
* [Example](#example)

<a name="installing"><h2>Installing</h2></a>
Add the package to your project
```
npm i hans-obj-comparator
```
using yarn
```
yarn add hans-obj-comparator
```

<a name="example"><h2>Example</h2></a>

Export *compareObjects* or *compareArrays* from *hans-obj-comparator*

```javascript
const {compareObjects, compareArrays} = require('hans-obj-comparator')
```
using TypeScript
```typescript
import {compareObjects, compareArrays} from 'hans-obj-comparator'
```  

```typescript
console.log(compareObjects({a: 2, b: [1, 2, 4]}, {a: 2, b: [1, 2, 4]})) // true
console.log(compareObjects({a: 2, b: [8, 2, 4]}, {a: 2, b: [1, 2, 4]})) // false
console.log(compareObjects({a: 2, name: 3}, {a: 2, b: 3})) // false

console.log(compareArrays([{a: 123, b: 2}, {a: 1, b: -2}], [{a: 123, b: 2}, {a: 1, b: -2}])) // true
console.log(compareArrays([1, 2], [1, 2, 3])) // false
console.log(compareArrays([], [1, 2, 3])) // false
```
