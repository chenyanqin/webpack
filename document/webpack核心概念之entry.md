## Entry的用法
- 单入口: entry是一个字符串
```
module.exports = {
  entry: './src/index.js'
}
```
- 多入口: entry是一个对象
```
module.exports = {
  entry: {
    app: './src/app.js',
    adminApp: './src/adminApp.js'
  }
}
```