## Javascript 代码风格

### 基本设置

- 2 空格缩进
- UTF-8 编码

### 引号

使用单引号，JS 内 html 相关使用双引号

### 严格模式

建议所有业务代码打开严格模式

```js
'use strict';
```

**禁止使用 `eval` 和 `with`**

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

使用 // 作为注释符，可以使用 /* */ 作为多行注释符。注释符号与注释内容之间留空，注释的位置尽量放在代码之上：

```js
/*not recommend*/
//not recommend
; // recommend

/* recommend */
// recommend
;
```

### 不要为大括号另开一行

```js
// not recommend
if (foo)
{
  // ...
}

// recommend
if (foo) {
  // ...
}

// not recommend
return
{
  a: 1
};

// recommend
return {
  a: 1
};
```

只有一行语句时允许不带括号，但需把语句紧跟当前行后

```js
if (foo) doSomething();
for (var i = 0; i < 10; i++) doSomething();
```

写 else 时不要另起一行

```js
// not recommend
if (test) {
  things1();
  things2();
}
else {
  things3();
}

// recommend
if (test) {
  things1();
  things2();
} else {
  things3();
}

```

