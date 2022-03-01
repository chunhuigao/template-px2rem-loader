## template-px2rem-loader

主要作用是将 vue 中 template 内连样式 px 转换为 rem

## 使用

### vue3.0

```js
module.exports = {
  chainWebpack: (config) => {
    config.module
      .rule('vue')
      .test(/\.vue$/)
      .use('template-px2rem-loader')
      .loader('template-px2rem-loader')
      .options({
        viewportWidth: 750,
        include: /HelloWorld/i,
      })
  },
}
```
