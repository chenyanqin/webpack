- webpack开箱即用只支持JS和JSON两种文件类型，通过Loaders去支持其它文件类型并且把它们转化成有效的模块，并且可以添加到依赖图中。
- 本身是一个函数，接受源文件作为参数，返回转换的结果。
  
```
const path = require('path');

module.exports = {
  ...,
  module: {
    rules: [
      { test: /\.txt$/, use: 'raw-loader'} // test: 指定匹配规则, use: 指定使用的loader名称
    ]
  }
}
```