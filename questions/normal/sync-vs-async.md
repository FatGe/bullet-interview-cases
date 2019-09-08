# JavaScript中的同步代码和异步代码有什么区别

## 参考答案

同步意味着每个操作必须等待前一个操作完成。

异步意味着在仍在处理另一个操作时可以进行操作。

在JavaScript中，由于它的单线程特性，所有代码都是同步的。但是，这不意味着异步操作（例如`XMLHttpRequest`或`setTimeout`）是在主线程之外处理的，它们还是由本机代码（浏览器API）控制的，异步程序的回调部分仍然会同步执行。

## 关键点

* JavaScript具有基于“事件循环”的并发模型;
* 像 `alert` 这样的函数会阻塞主线程，因此在用户关闭之前不会注册任何用户输入。

## 额外参考

<!-- tags: (javascript) -->
