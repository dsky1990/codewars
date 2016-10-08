## 素数
输入一个数字，判断是否为素数， 例如，input：3 ，output：true

```js
function isPrime(num) {
    for(var i = 2; i < num; i++) {
        if(num % i === 0) {
            return false;
        }
    }
    return num > 1;
}
```
