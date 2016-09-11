##降序
输入任何一个非负数的数字，将数字的顺序由大到小重新排列，例如Input: 1254859723 Output: 9875543221

```js
function descendingOrder(n){
  var str = ''+n;
  var orderArray = str.split('');
  var result = null;
  function sortNumber(a,b) {
    return b - a;
  }
  orderArray = orderArray.sort(sortNumber);
  result = Number(orderArray.join().replace(/,/g,''));
  return result;
}
```
优化后
```js
function descendingOrder(n){
  return parseInt(String(n).split('').sort().reverse().join(''));
}
```
