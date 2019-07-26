# 简单讲解一下http2的多路复用

## Answer

多路复用 (Multiplexing)，即连接共享，即每一个 request 都是是用作连接共享机制的。一个 request 对应一个 id，这样一个连接上可以有多个 request，每个连接的 request 可以随机的混杂在一起，接收方可以根据 request 的 id 将 request 再归属到各自不同的服务端请求里面。

将 HTTP/1.x 消息分为帧并嵌入到流中，数据帧与报头帧分离，这将允许头部压缩。将多个流组合，这是一个被称为 多路复用 (multiplexing) 的过程，它允许更有效的底层 TCP 连接。

## Good to hear

* HTTP/2 帧机制是在 HTTP/1.x 语法和底层传输协议之间增加了一个新的中间层，而没有从根本上修改它，即它是建立在经过验证的机制之上。

## Additional links

* [HTTP消息](https://developer.mozilla.org/zh-CN/docs/Web/HTTP/Messages)
* [HTTP,HTTP2.0,SPDY,HTTPS 你应该知道的一些事](http://www.alloyteam.com/2016/07/httphttp2-0spdyhttps-reading-this-is-enough/#prettyPhoto)

<!-- tags: (http) -->

<!-- expertise: (0) -->