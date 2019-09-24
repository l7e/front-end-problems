### 什么是BFC
1. 内部的块级元素会在垂直方向，一个接一个地放置；
2. 块级元素垂直方向的距离由margin决定。属于同一个BFC的两个相邻的块级元素会发生margin合并，不属于同一个BFC的两个相邻的块级元素不会发生margin合并；
3. 每个元素的margin box的左边，与包含border box的左边相接触（对于从左往右的格式化，否则相反）。即使存在浮动也是如此；
4. BFC的区域不会与float box重叠；
5. BFC就是页面上的一个隔离的独立容器，容器里面的子元素不会影响到外面的元素；外面的元素也不会影响到容器里面的子元素；
6. 计算BFC的高度时，浮动元素也参与计算。
### 创建BFC
1. loat的值不为none；
2. overflow的值不为visible；
3. position的值为fixed / absolute；
4. display的值为table-cell / table-caption / inline-block / flex / inline-flex。