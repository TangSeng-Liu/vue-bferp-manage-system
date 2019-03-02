# vue-bferp-manage-system #
基于Vue.js + Element UI ,借鉴#林鑫#的开源项目完善构建而成,感谢前辈们的付出！项目还在持续测试完善中...

## 前言 ##
之前在软件外包公司制作了很多网站的后台,很多功能模块都是可以直接复用的,所有我把常用的组件总结到了这个开源方案里面,基本适用于大部分的后台系统

主题的颜色是可以在scss自定义

## 目录结构介绍 ##


	|-- public                           // 公共文件
    |   |-- data                         // json数据
    |   |-- index.html                   // 入口html文件
	|-- src                              // 源码目录
	|   |--assets
	|       |-- css                      // css文件
    |       |-- img                      // 图片文件
	|   |-- components                   // 组件
	|       |-- bus.js           	     // Event Bus
	|       |-- Header.vue               // 公共头部
	|       |-- Home.vue           	     // 公共路由入口
	|       |-- Sidebar.vue              // 公共左边栏
	|       |-- Tags.vue           	     // 页面切换标签组件
	|   |-- page                   	     // 主要路由页面
	|       |-- 403.vue
	|       |-- 404.vue
	|       |-- BaseCharts.vue           // 基础图表
	|       |-- BaseForm.vue             // 基础表单
	|       |-- BaseTable.vue            // 基础表格
	|       |-- DashBoard.vue            // 系统首页
	|       |-- DragList.vue             // 拖拽列表组件
	|       |-- Icon.vue	             // 自定义图标组件
	|       |-- Login.vue          	     // 登录
	|       |-- Markdown.vue             // markdown组件
	|       |-- Premission.vue           // 权限测试组件
	|       |-- Upload.vue               // 图片上传
	|       |-- VueEditor.vue            // 富文本编辑器
	|   |-- App.vue                      // 页面入口文件
	|   |-- main.js                      // 程序入口文件，加载各种公共组件
	|-- .babelrc                         // ES6语法编译配置
	|-- .editorconfig                    // 代码编写规格
	|-- vue.config                       // cli-3配置文件
	|-- package.json                     // 项目及工具的依赖配置文件
	|-- README.md                        // 说明


## 安装步骤 ##

	git clone https://github.com/TangSeng-Liu/vue-bferp-manage-system.git      // 把模板下载到本地
	cd vue-manage-system    // 进入模板目录
	npm install         // 安装项目依赖，等待安装完成之后

## 本地开发 ##

	// 开启服务器，浏览器访问 http://localhost:8080
	npm run dev

## 构建生产 ##

	// 执行构建命令，生成的dist文件夹放在服务器下即可访问
	npm run build

## 组件 ##

### element-ui ###
一套基于vue.js2.0的桌面组件库。访问地址：[element](http://element.eleme.io/#/zh-CN/component/layout)

### Vue-Quill-Editor ###
基于Quill、适用于Vue2的富文本编辑器。访问地址：[vue-quill-editor](https://github.com/surmon-china/vue-quill-editor)

（IE10及以下不支持）

### mavonEditor ###
基于Vue的markdown编辑器。访问地址：[mavonEditor](https://github.com/hinesboy/mavonEditor)

### vue-cropperjs ###
一个封装了 cropperjs 的 Vue 组件，用于裁剪图片。访问地址：[vue-cropperjs](https://github.com/Agontuk/vue-cropperjs)


## 如何切换主题色呢？ ##

 1、修改src/assets/css/theme/element-variables.scss中$color变量色值即可改变整体主题颜色 
 
 2、头部菜单如果需要单独配色修改element-variables.scss中.header中的背景颜色 
 
3、菜单颜色在src/components/Sidebar.vue中修改el-menu标签上的background-color(背景色)、text-color(字体颜色)、active-text-color(选中颜色)三个属性 

