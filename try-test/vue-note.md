# cute points
- 可以用 v-model 指令在表单控件元素上创建双向数据绑定，但 v-model 本质上不过是语法糖。
- syntactic sugar，增加程序可读性，减少代码出错机会，方便程序员使用，广义的理解，从面向过程到面向对象也是一种语法糖，如果生硬的照此理解，只有计算机硬件指令才不算语法糖，所以语法糖这个词绝非贬义词。
- label标签的for，绑定的是元素的ID值。
- 和表单v-model相关的一些修饰符
```html

<!-- .lazy "input" 事件中不更新 -->
<input v-model.lazy="msg" >

<!-- 如果要自动过滤用户输入的首尾空格，可以添加 trim 修饰符到 v-model 上 -->
<input v-model.trim="msg">


```

- 要确保在初始化根实例之前注册了组件
```javascript
// 注册
Vue.component('my-component', {
  template: '<div>A custom component!</div>'
})
// 创建根实例
new Vue({
  el: '#example'
})

//也可以局部注册
var Child = {
  template: '<div>A custom component!</div>'
}
new Vue({
  // ...
  components: {
    // <my-component> 将只在父模板可用
    'my-component': Child
  }
})
```
- vue模板语法
```javascript
//mustache语法不能在HTML属性中使用，应使用v-bind
```
- 重新梳理  
关于vue的兼容性：vue.js不支持IE8及其以下版本。  
v-for指令：绑定数组。





















