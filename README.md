# vue-demo01

> vue-demo01

## Build Setup
此demo使用axios(第三方请求数据插件)请求mock.js自动生成的数据。

Vue.prototype.$http = axios  在main.js中把axios添加到vue原型中，则可在每个组件中调用
//全局引入使用vue原型中的方法this.$http,已经把axios添加到原型中

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
