# localStorage基本用法
``` javascript
let value = '哈哈';
localStorage.setItem('haha', value);
let getVal = localStorage.getItem('haha');
console.log(getVal); // 哈哈

```
or
``` javascript
let value = 'hello啊';
localStorage.sayHello = value;
let getVal = localStorage.sayHello;
console.log(getVal); // hello啊

```
保存JSON格式

``` javascript 
let value = [
  {
    name: 'weikexin',
    age: 18,
    sayHello () {
	  console.log('WTF');
	}
  }
];
localStorage.setItem('userInfo', JSON.stringify(value)); // 注意 是,隔开
let getVal = localStorage.getItem('userInfo');
console.log(getVal); // "[{"name":"weikexin","age":18}]"
console.log(typeof getVal); // string
console.log(JSON.parse(getVal)); // [{"name":"weikexin","age":18}]
console.log(typeof getVal); // object

```
注意 在`setItem`的时候记得要加`JSON.stringify()` 不然直接`getItem`时是个字符串 没法直接使用 加上`JSON.parse()`会报错 所以存的时候要`stringify` 取的时候要`parse`

完全个人想法 可能会有错误