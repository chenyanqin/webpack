- Output用来告诉webpack如何将编译后到文件输出到磁盘

```
module.exports = {
  entry: {
    index: './src/index.js',
    search: './src/search.js'
  },
  output: {
    path: path.join(__dirname, 'dist'),
    filename: '[name].js' // 通过占位符确保文件名称的唯一
  },
  mode: 'production'
};
```