<p align="center">
    <a href="http://www.maxiaoqu.com/">
        <img width="300" src="http://www.maxiaoqu.com/maxiaoqu.png">
    </a>
</p>

<h2>
    vue-selecttree
    <h4>一个很好用的Vue多功能树组件</h4>
</h2>

## 相关链接
- [案例地址](http://github.maxiaoqu.com/vue-selecttree/)
- [api文档](http://blog.maxiaoqu.com/packagesApi/)
- [demo地址](https://github.com/maxiaoqu/vue-selecttree-demo/)
- [npmjs插件](https://www.npmjs.com/package/vue-selecttree/)

## 在main.js使用
```js
import Vue from 'vue';
import vueSelecttree from 'vue-selecttree';

Vue.use(Vue)
Vue.use(vueSelecttree)
```

## vue文件里使用方法
```vue
<template>
    <vue-selecttree :data="data" :props="defaultProps"></vue-selecttree>
</template>
<script>
    export default {
        data () {
            return {
                defaultProps: {
                    children: 'children',
                    label: 'label'
                },
                data: [{
                      label: "一级 1",
                      name: "一级 1 000",
                      children: [{
                          label: "二级 1-1",
                          name: "二级 1-1 000",
                          children: [{
                              label: "三级 1-1-1",
                              name: "三级 1-1-1 000"
                          }]
                      }]
                    },{
                        label: "一级 2",
                        name: "一级 2 000",
                        children: [{
                            label: "二级 2-1",
                            name: "二级 2-1 000",
                            children: [{
                                label: "三级 2-1-1",
                                name: "三级 2-1-1 000"
                            }]
                        }]
                    }]
            }
        }
    }
</script>
```

## 主要维护人员
|人员|github账号|头像|作者网站|联系邮箱|
|---|---|---|---|---|
|杨正炳|[maxiaoqu](https://github.com/maxiaoqu) |  ![](https://avatars1.githubusercontent.com/u/25891598?s=60&v=4)|www.maxiaoqu.com|maxiaoqu@gmail.com

## 安装
```
npm install
```

## 运行
```
npm run serve
```

## 打包
```
npm run build
```

## 检查
```
npm run lint
```