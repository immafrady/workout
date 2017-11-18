# 知识点

### 1. `this`的指向

构造函数`Model`里的`this`，和`Model.prototype.function`的指向是一样的。

但是，假若`Model.prototype.function`内又包裹了函数，那么必须要借助第三个指针把`this`引进去。

这就是`let that = this`的由来

### 2. `clear`与`set`

`clearTimeout/clearInterval`可以在`setTimeout/setInterval`内部包裹的函数执行，消除自身印象。

简称“自爆”?

###