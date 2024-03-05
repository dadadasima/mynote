### Component

```jsx
const App = () => (
  <div>
    <p>Hello world</p>
  </div>
)


() => {
  <div>
    <p>Hello world</p>
  </div>
}
//一个JavaScript函数

ReactDOM.createRoot(document.getElementById('root')).render(<App />)
```

App.js中定义了一个名为APP的**React组件**

render()方法：接受输入的数据并返回需要展示的内容

### JSX

~~React组件返回的是HTML标记~~。事实上，React组件的布局大多是用JSX编写的。

在使用JSX时，你可以通过在大括号内编写适当的JavaScript来嵌入动态内容。



