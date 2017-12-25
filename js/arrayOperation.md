# JS数组操作
 `push()`  向数组的末尾添加一个或多个元素,并返回新的长度 
* 代码后的注释为返回值
``` javascript
let arrObj = [];
arrObj.push(variable1,variable2,variable3,'string1'); // arrObj.length
console.log(arrObj); // [variable1,variable2,variable3,'string1']
```

它会直接修改arrayObject,而不是创建新的数组

------

`pop()`  会删除数组的最后一个元素 并返回它删除的元素的值 
如果数组已经为空 则不改变数组 并返回`undefined`
```javascript
// 懒得敲那么多代码了 就接着用上一段的代码
arrObj.pop(); // string1
console.log(arrObj); // [variable1,variable2,variable3]

````
-----
`shift` 则删除数组的第一个元素 并返回被删除的元素
```javascript
arrObj.shift(); // variable1
console.log(arrObj); // [variable2,variable3]
```
----
`unshift` 向数组的开头添加一个或多个元素 并返回新的长度  会直接修改arrayObject
改方法的第一个参数将成为新的数组的第`[0]`未 如果有第二个参数则成为新数组的第`[1]`位 以此类推
```javascript
arrObj.unshift(variable1,variable2); //4
console.log(arrObj);// [variable1,variable2,variable2,variable3] 
```
-----
未完待续...