---
title: vue3学习
---
### 学习视频
[地址](https://www.bilibili.com/video/BV1Za4y1r7KE/?p=60&spm_id_from=pageDriver&vd_source=d089cf3fa472afb9fc2615b1cfc081f3)

```
1、vite-plugin-vue-setup-extend
2、volar插件可以解决ref变量必须使用.value问题
3、ref能处理对象跟基本类型，reactive只能处理对象。ref处理对象的底层也是使用reactive
4、想整体修改reactive所定义的数据，需要使用Objece.assign()
5、toRefs与toRef
6、watch（谁--》可以是写对象，(newValue,oldValue),{deep:true,immediate:true}）
7、reactive定义的属性，watch监听是深度监听，且不能关闭的
8、watchEffect,灵活度高，不需要指明监听谁
9、组件标签中，子给父的值defineExpose
10、defineProps([])、defineProps<>()、whitDefaults(defineProps<>(),{})
11、hooks，文件都需要以use开头
12、nanoid生成id工具13
13、pinia。变更方法1）直接修改2）$patch 3)actions-->主要用于复用
14、pinia中的storeToRefs、$subscribe()->数据变化的订阅监听
15、$event、defineEmits
16、订阅发布（总线）：mitt，pinia
17、$attrs
18、defineExpose、$refs、$parent
19、provide与inject向后代提供数据
20、默认插槽、具名插槽、作用域插槽（父亲想要数据，但是数据在孩子那）
21、shallowRef、shallowReactive
22、readonly、shallowReadonly
23、toRaw（不是响应式）\markRaw(永远不会是响应式数据)

````