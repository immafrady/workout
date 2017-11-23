# 备忘录

### 1.CSS选择器：兄弟选择符 “~”妙用
---
兄弟选择符是被选中的选择器后每个符合条件的同级元素。

所以想做的指针跟随鼠标移动的话，可以在列表末尾设定一个块状元素，通过兄弟选择器去调用它。

### 2.`flex-box`
---
#### `justify-content`
* `flex-direction`为`row`的前提下：`flex-start`为左边；
* `flex-direction`为`row-reverse`的前提下：`flex-start`为右边；
* `flex-direction`为`column`的前提下：`flex-start`为上边；
* `flex-direction`为`column-reverse`的前提下：`flex-start`为下边；

#### `align-self`和`align-items`、`align-content`的区别
* `align-self`用于flex的**子项**，单独调试每个子项的位置；
* `align-items`用于flex的**母项**，统一调试盒子内部每一个子项的位置（不改变子项的样式）；
* `align-content`用于flex的**母项**，统一改变盒子内部每个子项的样式，使到子项盒子达到统一样式


奇特现象，在本例中，用`align-item`，虽说也是内容居中了，但是`ul`盒子会被拉到撑满整个盒子；
而在`ul`上用`align-self`，实际上是把整个盒子位移了
