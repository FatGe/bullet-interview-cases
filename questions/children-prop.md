### `children` 属性的作用什么?

#### Answer

`children`是传递给组件的props对象的一部分，它允许将组件作为数据传递给其他组件，从而提供了优雅地组合组件。React API中有许多方法可用于此prop，例如`React.Children.map`, `React.Children.forEach`, `React.Children.count`, `React.Children.only` 以及 `React.Children.toArray`。

```js
function GenericBox({ children }) {
  return <div className="container">{children}</div>
}

function App() {
  return (
    <GenericBox>
      <span>Hello</span> <span>World</span>
    </GenericBox>
  )
}
```

#### Good to hear

* Children是一个prop，可以将组件作为数据传递给其他组件。
* React API提供了使用此prop的方法。