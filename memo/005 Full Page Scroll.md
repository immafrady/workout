# 备忘录

### 1. 各家浏览器对Scroll Action的适配（基于jQuery）
---
##### Chrome系（包括Opera）、IE系（包括Edge）
>取`wheelDelta`值（一步为120，向下为负）

    $(window).on('mousewheel',function(event){
        return event.originalEvent.wheelDelta
    }

##### Firefox
>取`detail`值（一步为3，向下为正）

    $(window).on('DOMMouseScroll',function(event){
        return event.originalEvent.detail
    }

### 2. `body`与`html`的配置

在`body`上用`position:absolute`，千万不要用在`html`上，否则只能显示第一屏，其它颜色都是不会显示出来

### 3. 滚的方向
---
注意，由于是往下滚，所以方向都要留意一下啊。

### 4. 关于`top`值
---
由于基准点是页面顶部，所以最后那页的顶部其实是倒数第二页的尾部。
所以

### 5. 其他人的解决方案

[前端开发——滚滚屏（没有纵向滚动条）](http://blog.csdn.net/luohuaxinyue/article/details/51068034)