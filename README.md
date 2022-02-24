# @jzo/babel-plugin-bin

## 安装
```
npm install @jzo/babel-plugin-bin --save-dev
```
### 使用说明
```
// .babelrc
"plugins": [
    [
      @jzo/babel-plugin-bin",
      {
        "library": "yournpm" // 支持数组["yournpm", "yournpm2"]
      }
    ],
  ]
  
### 注意
打包规则必须在bin目录下面  
  
  
// index.js
import { 组件名称 } from '包名';

      ↓ ↓ ↓ ↓ ↓ ↓

var _helloworld = require('包名/lib/组件名称');
```


