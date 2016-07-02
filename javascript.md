## Javascript 代码风格

### 基本设置

- 2 空格缩进
- UTF-8 编码

### 严格模式

建议所有业务代码打开严格模式

```js
'use strict';
```

### 分号

在语句（Statement）的结尾加分号

```js
// not recommend
var fn = function() {

} // without semicolon

// recommend
var fn = function() {

}; // with semicolon
```

### 空白与格式

在二元和三元运算符的符号与操作数之间添加空格，在非行末的 `,` `;` `}` 后添加空格，在 `{` 前添加空格。并在每个逻辑块中间添加空白行。
特别的，在 if、while 等关键字后加空格，与函数调用做区分。function 后不加空格

```js
// not recommend
var a=1,b=2;
function foo () {}
if(aa&bb) {
  
}else{}

// recommend
var a = 1;
var b = 2;

if (aa & bb) {

} else {

}
```

### 注释


