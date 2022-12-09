### 正则表达式范例

##### 只能输入串纯数字，小数点不可以

```js
<input type="text" οnkeyup="value=value.replace(/[^\d]/g,'')" > 
```

<input type="text" οnkeyup="value=value.replace(/[^\d]/g,'')" > 

##### 保留两位小数

```js
<input type="text" οnkeyup="value=value.replace(/^\D*(\d*(?:\.\d{0,2})?).*$/g, '$1')" >
```

<input type="text" οnkeyup="value=value.replace(/^\D*(\d*(?:\.\d{0,2})?).*$/g, '$1')" > 

##### 保留一位小数

```js
<input type="text" οnkeyup="value=value.replace(/^\D*(\d*(?:\.\d{0,1})?).*$/g, '$1')" > 
```

<input type="text" οnkeyup="value=value.replace(/^\D*(\d*(?:\.\d{0,1})?).*$/g, '$1')" > 

#####  第一位不为0，且不能输入小数

```js
<input type="text" οnkeyup="value=value.replace(/[^\d]/g,'').replace(/^0{1,}/g,'')" >
```

<input type="text" οnkeyup="value=value.replace(/[^\d]/g,'').replace(/^0{1,}/g,'')" >
————————————————
原文链接：https://blog.csdn.net/weixin_39677942/article/details/119951959

### 正则表达式  

#### 常用函数

##### sort（升序降序）

```javascript
//数字升序
var points = [40,100,1,5,25,10];
points.sort(function(a,b){return a-b});
//数字降序
points.sort(function(a,b){return b-a});
//若数组的元素是数组，按元素的第一个数排升序
let reArr=[[0,1],[2,2],[3,3],[1,4]]
reArr.sort((a,b)=>a[0]-b[0]);//[[0,1],[1,4],[2,2],[3,3]]

```



