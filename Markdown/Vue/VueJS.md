# VueJS

一套用于构建用户界面的__渐进式框架__



## MVVM

![](https://gitee.com/code-shuai/map-depot/raw/master/VueJS/MVVM.png "Vue - MVVM")







## 一、Vue 基础语法



### 插值操作

**常见指令**

#### 1. Mustache 语法

```
{{Mustache}} 胡子/胡须
```

```
<div id="app">
	<h1>{{name}}</h1>
	<h1>{{age +" | "+ sex}}</h1>
	<h1>{{age}} | {{sex}}</h1>
	<h1>{{age + 1}}</h1>
</div>
<script>
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三",
				age: 18,
				sex: "男"
			}
		}
	})
</script>
```

#### 2. v-once 

```
<div id="app">
	<i>{{name}}</i>
	<!-- 动态数据发生改变，使用 v-once 不会改变 -->
	<h1 v-once>{{name}}</h1>
</div>
<script>
	new Vue({
		el: "#app",
		data: function(){
			return{
				name: "张三"
			}
		}
	})
</script>
```
#### 3. v-html

```
<div id="app">
	<i>{{name}}</i>
	<!-- 遇到可识别文字时使用 -->
	<h1 v-html="url">{{name}}</h1>
</div>
<script>
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三",
				url:"<a href="baidu.com">百度</a>"
			}
		}
	})
</script>
```

#### 4. v-text

```
<div id="app">
	<!-- 尽量不要使用 v-text 不够灵活 -->
	<h1>{{name}}</h1>
	<h1 v-text="name"></h1>
</div>
<script>
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三",
				url:"<a href="baidu.com">百度</a>"
			}
		}
	})
</script>
```


#### 5. v-pre

```
<div id="app">
	<h1>{{name}}</h1>
	不需要vue 解析
	<h1 v-pre>{{name}}</h1>
</div>
<script>
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三",
				url:"<a href="baidu.com">百度</a>"
			}
		}
	})
</script>
```

#### 6. v-cloak


```
<style type="text/css">
	[v-cloak]{
		display: none;
	}
</style>
<div id="app">
	<h1>{{name}}</h1>
	<!-- 特殊情况处理（当js未读取到时） -->
	<!-- 防止闪动 -->
	<h1 v-cloak>{{name}}</h1>
</div>
<script>
	setTimeout(function(){
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三"
			}
		}
	})
	},1000)
</script>
```



### 绑定属性

#### 1. v-bind

##### 基础操纵
```
<!-- v-bind 基础使用 -->
<div id="app">
	<!-- {{}} 只能使用在<>内部</> -->
	<i>{{name}}</i>
	<!-- 动态绑定至**属性** -->
	<img v-bind:src="imgUrl" >
	<a v-bind:href="aHref">百度</a>
	<!-- 语法糖 -->
	<img :src="imgUrl" >
	<a :href="aHref">百度</a>
</div>
<script>
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三",
				imgUrl:"https://gitee.com/code-shuai/map-depot/raw/master/bilibili/bilibili_1001.webp",
				aHref:"baidu.com"
			}
		}
	})
</script>
```

**进阶操作**

##### 对象语法

```
<style>
	.active{
		color: red;
	}
	.line{
		color: blue;
	}
</style>
<!-- 对象语法 -->
<div id="app">
	<i>{{name}}</i>
	<h1 :class="active"></h1>
	<!-- v-bind 可放对象 -->
	<!-- <h1 :class="{类名1:true,类名2:false}"></h1> -->
	<h1 :class="{active:true,line:false}">{{name}}</h1>
	<h1 :class="{active:isActive,line:isLine}">{{name}}</h1>
	<h1 class="title" :class="{active:isActive,line:isLine}">{{name}}</h1>
	<button type="button" v-on:click="btnClick">dian</button>
</div>
<script>
	new Vue({
		el: "#app",
		data: function() {
			return {
				name: "张三",
				active:"active",
				line:"line",
				isActive:true,
				isLine:false
			}
		},
		methods:{
			btnClick:function(){
				this.isActive = !this.isActive;
			}
		}
	})
</script>
```

##### 数组语法




### 计算属性

### 事件监听

### 条件判断

### 循环遍历

### 阶段案例

### v-model






## 二、组件化开发

## 三、Vue CLI 详解

## 四、Vue-router

## 五、Vuex 详解

## 六、网络封装


