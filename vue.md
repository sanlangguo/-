### vue 面试总结

* vue响应式原理

  [vue官网解释](https://cn.vuejs.org/v2/guide/reactivity.html)


* vue文件编译原理
 
  [参考链接](https://forum.vuejs.org/t/vue-js-vue-js/60884)

* 计算属性 VS 监听属性
 
  ```
  watch：监测的是属性值， 只要属性值发生变化，其都会触发执行回调函数来执行一系列操作。
  computed：监测的是依赖值，依赖值不变的情况下其会直接读取缓存进行复用，变化的情况下才会重新计算。

  计算属性适合用在模板渲染中，某个值是依赖了其它的响应式对象甚至是计算属性计算而来；而侦听属性适用于观测某个值的变化去完成一段复杂的业务逻辑。
  ```