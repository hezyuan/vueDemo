# demo

<a href="https://996.icu"><img src="https://img.shields.io/badge/link-996.icu-red.svg" alt="996.icu" /></a>

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev

# build for production with minification
npm run build

# build for production and view the bundle analyzer report
npm run build --report
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).

主要测试组件通信分为三个方面：
1.父组件传递数据给子组件，分两种方式
 #子组件触发获取父组件的数据，如子组件里点击按钮获取父组件数据
 #父组件触发，子组件获取父组件数据

 2.子组件传递数据给父组件，方式和父到子一新

 3.兄弟组件之前传递数据

