# DOM节点操作

标签： DOM

---

## 子节点：
- childNodes：包含了文本内容；
- children：包含了节点，不包含文本内容；

- firstChild：获得标签的首个子节点，首个节点是文本节点；
- lastChild：获得标签的最后一个子节点，最后一个节点是文本节点；

- firstElementChild：获得标签的首个元素节点；
- lastElementChild：获得标签的最后一个元素节点；

## 当前节点的名称：nodeName
## 当前节点的类型：nodeType

## 获得当前节点的父节点：parentNode

## 创建节点：
- 方法：document.createElement(节点);
- 注意：创建好了之后还要添加到相应的标签里面；

## 添加节点：放到父节点中成为最后一个子节点；
- 方法：父节点.appendChild(要添加的节点);

## 在前面插入节点：
- 方法：父节点.insertBefore(要添加的节点,谁之前);

## 替换节点：
- 方法：父节点.replace(要替换的节点,被替换的节点);

## 位置：
```
offsetLeft
offsetTop
```
> 注意：offsetLeft / offsetTop不包含外边框，也就是外边框之外，设置了margin对它们没什么影响；

```
offsetWidth
offsetHeight
```
> 注意：offsetWidth / offsetHeight不包含margin，外边框包含在内。

```
clientWidth
clientHeight
```
> 注意：clientWidth / clientHeight不包含外边框，也不包含margin，但包含padding；

```
scrollWidth
scrollHeight
scrollLeft
scrollTop
```