# san-webpack-loader
🌈 a webpack-v4 loader for San.js ☄️

## 重写的初衷 AOT vs JIT
1. 避免运行时编译的代价
2. 避免把编译器发送到浏览器里
3. 极致的开发体验和效率

## 相比san-loader:

1. 构建后的san组件业务代码体积缩小60%
2. 相比san-loader复杂的配置项，零配置&&开箱即用
3. 业务组件script时间减少30%
4. 组件级别热重载
5. 通过template literal静态连接模板和js
6. 更少的构建时间

## todo
1. webpack4 Boilerplate 多线程优化
2. css in js 方案

## 目标
1. 极小的产出体积
2. 更快的运行时解析
3. 零配置
4. 更好的开发体验
5. 有文档 📖
6. 更好的业务服务集成

## 设计
1. css仅支持原生css/stylus/postcss，支持1个 `<style>`标签，一个scoped 一个全局
2. esModule only, babel-loader转码
3. template 仅支持原生html模板
4. 组件级别热重载 ？？
5. `scoped`组件模拟css作用域 【已废弃】
6. 导出对象为Object对象/Component?
7. template 支持template expression
8. css in js 方案？
9. 语法检查集成？
