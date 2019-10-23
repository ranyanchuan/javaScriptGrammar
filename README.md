# javaScriptGrammar


1.下面哪个选项打印出的来值不为{}? (**D**)
```
  A. console.log({...true})
  B. console.log({...undefined})
  C. console.log({...null})
  D. console.log({...'hello'})
```
2.let aClone={...a}; 与 let aClone=Object.assign({},a);是否等价?(**A**)
``` 
  A. 等价
  B. 不等价
  C. 等不等价由a决定
```
3.await 命令后只能返回一个Promise对象吗？(**B**)
```
  A. 只能返回Promise对象
  B. 可以返回任意类型
```
4.下面哪些选项打印出来的值不为true？(**B,C,D**)
```
  A. console.log(1=='1')
  B. console.log(NaN===NaN)
  C. console.log(1==='1')
  D. console.log(1===true)
```
5.Number('0.010')的值为多少？(**A**)
```
  A. 0.01
  B. 0.010
  C. 0.0
  D. 0
```
6.下面哪些选项的打印值不为8? (**C,D**)
```
  A. console.log(2***3)
  B. let a=2; a**=3; console.log(a)
  C. let a=2; a**=4; console.log(a)
  D. console.log(2**1**2)
```

7.下面哪个选项打印值为false？ (**B**)
```
  A. console.log([1,2,3].includes(2))
  B. console.log([1,2,3].includes(4))
  C. console.log([1,2,NaN].includes(NaN))
  D. console.log([1,2,3].includes(3,-1))
```
8.下面console.log()打印出来的值是多少？(**{}**)
```
const json={}
const {size = 10, pageIndex = 0} = json;
delete json.size;
delete json.pageIndex;
console.log(json)
```
9. 用对象收编变量
```js
var CheckObject = {
        checkName: function () {
            return this;
        },
        checkEmail: function () {
            return this;
        },
        checkPassword: function () {
            return this;
        },
};

```
10. 递归改成For 循环
```js
    //  楼梯问题
    function jump(n){
        if(n===1) return 1;
        if(n===2) return 2;
        return jump(n-1)+jump(n-2);
    }

    // 使用循环
    function jumpFor(n){
        if(n===1) return 1;
        if(n===2) return 2;
        let ret =0;
        let pre = 2;
        let prepre = 1;

        for(let i=3;i<=n;i++){
            ret = pre + prepre;
            prepre = pre;
            pre = ret;
        }

        return ret;

    }

```

