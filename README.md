# vue2+vite

使用vite搭建的一个vue2 demo

引入了 `@vue/composition-api` 插件

和一些简单的 `eslint` & `prettier` 配置

## 搭建方法

以`Yarn`为例

搭建一个Vite项目，详见[官方文档](https://cn.vitejs.dev/guide/#scaffolding-your-first-vite-project)
``` shell
$ yarn create vite
```
然后按提示操作！

Vite 默认没有提供对 Vue2 的支持，所以我们在创建项目时，选择模版为`vanilla`，即原生js

// todo


先安装一个插件 `vite-plugin-vue2`
``` shell
$ yarn add vite-plugin-vue2 -D
```

然后在 `vite.config.js` 文件引入插件：
```js vite.config.js
import { defineConfig } from 'vite'
import { createVuePlugin as Vue2 } from 'vite-plugin-vue2'

export default defineConfig({
  plugins: [Vue2()]
})
```