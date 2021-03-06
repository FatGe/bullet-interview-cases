# `img` 标签上 `alt` 属性代表了什么

## 参考答案

这个属性定义了描述图像的替换文本。用户将看到这个显示，如果图像的URL是错误的，该图像不在**支持的格式**列表中，或者如果图像还没有被下载。

## 关键点

- 省略这个属性表明该图像是内容的关键部分，但没有等效的文本可用；
- 把这个属性设置为空字符串，表明该图像不是内容的关键部分，非可视化浏览器在渲染的时候可能会忽略它；
- Web 爬虫使用 `alt` 标签来理解图像内容，因此它们被认为对搜索引擎优化（SEO）很重要；
- 将 `.` 放在 `alt` 标记的末尾以提高可访问性。

## 额外参考

- [A good basis for accessibility](https://developer.mozilla.org/en-US/docs/Learn/Accessibility/HTML)

<!-- tags: (html) -->