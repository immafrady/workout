# 知识点

### 1. `this`的指向

构造函数`Model`里的`this`，和`Model.prototype.function`的指向是一样的。

但是，假若`Model.prototype.function`内又包裹了函数，那么必须要借助第三个指针把`this`引进去。

这就是`let that = this`的由来

### 2. `prototype`中的`this`指向

`Model.prototype.function` 内部指定的`this`层级与`Model`是相等的，可以在其他`prototype.function`里引用。

### 3. `clear`与`set`

`clearTimeout/clearInterval`可以在`setTimeout/setInterval`内部包裹的函数执行，消除自身印象。

简称“自爆”?

### 4. 注意阻止`form`的默认行为

否则会刷新网页