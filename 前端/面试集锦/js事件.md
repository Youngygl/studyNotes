# 事件绑定的几种方式

1. 在DOM元素中直接绑定；
2. 在JavaScript代码中绑定；
3. 绑定事件监听函数。

# 事件的冒泡与捕获

## 什么是事件流

事件流描述的是从页面中接受事件的顺序，但有意思的是，微软（IE）和网景（Netscape）开发团队居然提出了两个截然相反的事件流概念，**IE的事件流是事件冒泡流(event bubbling)，而Netscape的事件流是事件捕获流(event capturing)。**

## 事件冒泡

IE提出的事件流叫做事件冒泡，即事件开始时由**最具体的元素接收，然后逐级向上传播到较为不具体的节点**

## 事件捕获

网景公司提出的事件流叫事件捕获流。

事件捕获流的思想是不太具体的DOM节点应该更早接收到事件，而最具体的节点应该最后接收到事件



**DOM事件流**

 ‘DOM2级事件’规定的事件流包含3个阶段，**事件捕获阶段、处于目标阶段、事件冒泡阶段**。

https://www.cnblogs.com/christineqing/p/7607113.html