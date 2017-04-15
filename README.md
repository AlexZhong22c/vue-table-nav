> 原博文：https://alexzhong22c.github.io/2017/04/15/vue-table-nav/
>
>  [demo](https://alexzhong22c.github.io/vue-table-nav/vue-table-nav.html) (在线演示初次加载会有点慢，请稍等)

vue.js的出现，导致很多小插件的简单实现成为可能。

这是一个关于表格数据的分页导航，按照表格中的每个条目作为单元来展示数据。

**这样的数据呈现方式可读性更强，设计更人性化。**

当然它只适用于少量表格数据的直观呈现，如果数据太多，还是用传统的表格来呈现比较合适。demo的下方我还展示了原始的表格，方便各位看官做做对比。

![](http://olqa2s510.bkt.clouddn.com/show-vue-table-nav.png)

## 分页导航

- 可设置每页显示的条目数
- 用vue的 计算属性 和对象数组的slice()实现分页显示，非常简便
- 在总页数比较多的情况下仍能维持导航样式的统一

## 引用boostrap的样式

- css写得比较潦草，让大家见笑
- 对于class="pagination"，直接从bootstrap库复制了那部分的css样式

## 用dl dt dd标签展示键值对

- 阻止dt标签之后的换行
- 阻止dd标签之前的空白
- **为了方便阅读，直接用中文作为键值对的键名。在实际工程中当然不能这样。**

## 最后：

> 如果各位看官喜欢的话留一个Star吧！