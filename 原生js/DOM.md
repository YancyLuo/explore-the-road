## 1.常见的节点类型(nodeType)
- NODE.ELEMENT_NODE === 1
- NODE.ATTRIBUTE_NODE === 2
- NODE.TEXT_NODE === 3
- NODE.DOCUMENT_NODE === 9
- NDOE.DOCUMENT_FRAGMENT_NODE === 11
- NODE.COMMENT_NODE === 8

## 2.节点关系属性(注意文本节点)
- firstChild
- lastChild
- nextSibling
- previousSibling
- parentNode
- ownerDocument
- hasChildNodes()

- childElementCount
- firstElementChild
- lastElementChild
- nextElementSibling
- previousElementSibling
- children

- contains()：检测传入节点是否是调用节点的后代
* compareDocumentPosition():返回值：
  ** 1：无关
  ** 2：给定节点位于调用节点之前
  ** 4：给定节点位于调用节点之后
  ** 8：给定节点是调用节点的祖先
  ** 16：给定节点是调用节点的后代

## 3.操作节点
- appendChild()
- insertBefore()
- replaceChild()
- removeChild()
- cloneNode()
- insertAdjacentHTML()注意：第二个参数是一个HTML字符串
- normalize(): 合并相邻的文本节点并删除空的文本节点。

## 4.查找节点
- document.getElementsByTagName()
- document.getElementById()
- getElementsByClassName()
- getElementsByName()
- querySelector()
- querySelectorAll()
- 特殊集合：document.anchors、document.forms、document.images、document.links

## 5.创建元素
- document.createElement()
- document.createTextNode()
- document.createAttribute()
- document.createComment()
- document.createDocumentFragment()

## 6.节点大小
- 偏移量：offsetHeight、offsetWidth、offsetTop、offsetLeft(都为只读)
- 客户区大小：clientWidth、clientHeight，元素内部空间的大小（不含边框）
- 滚动大小： scrollWidth、scrollHeight，scrollLeft、scrollTop
- getBoundingClientRect()

## 7.节点遍历
* NodeIterator
  ** nextNode()、previousNode()

* TreeWalker
  ** nextNode()、previousNode()
  ** parentNode()、firstChild()、lastChild()、nextSibling()、previousSibling()

注意： 第一次调用nextNode()时，如果根节点满足条件，NodeIterator会输出根节点TreeWalker会输出满足条件的下一个节点



