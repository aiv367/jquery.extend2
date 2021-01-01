# jquery.extend2
功能跟jQuery.extend基本一致，唯一区别是，extend2 针对 array 类型数据，是采用覆盖赋值方式，而不是追加合并方式。

## 引入

``` html
<script src="./jquery.min.js"></script>
<script src="../src/jquery.extend2.js"></script>
```

## 示例

``` javascript
let a = {
	data: [1, 2, 3]
};

let b = {
	data: [4, 5, 6]
};

let c =  $.extend2(true, a, b);

//结果
c = {
	data: [4, 5, 6]
}

//如果是原始jquery.extend 方法会返回下面结果
c = {
	data: [1, 2, 3, 4, 5, 6]
}
```