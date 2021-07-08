# 一、 Vue核心

## 1.1初识Vue

## 1.2Vue模板语法

标签、标签属性、标签体

<img src="C:\Users\17645\AppData\Roaming\Typora\typora-user-images\image-20210705190544194.png" alt="image-20210705190544194" style="zoom:33%;" />

- 插值语法：

  - 功能：解析==标签体==功能，向==标签体==中插入值！
  - 写法：{{xxx}}，xxx作为==表达式==去解析，自动读取data中属性

- 指令语法

  - 功能：解析标签（标签属性、标签内容、绑定事件）

  

  ```html
  <!-- 指令语法 -->
  <!-- url自动读取data中属性 -->
  <a v-bind:href="url">百度一下</a>
  <a :href="url">百度一下</a>
  ```

  只有`v-bind:`指令能简写成`:`

1.3数据绑定

<img src="C:\Users\17645\AppData\Roaming\Typora\typora-user-images\image-20210706085930873.png" alt="image-20210706085930873" style="zoom:33%;" />



​    1.单向数据绑定（v-bind）：数据只能从data流向页面

​    2.双向数据绑定（v-model）：数据不仅能从data流向页面，还能从页面流向data

​    备注：

​      1.双向数据绑定一般针对表单类元素（输入类的值，可以产生交互）

​      2.v-model:value可以简写为v-model:  因为v-model默认收集value值



### 什么是MVVM？

- 概念介绍

  - MVVM分为三个部分：分别是M（Model，模型层 ），V（View，视图层），VM（ViewModel，V与M连接的桥梁，也可以看作为控制器）
     1、 M：模型层，主要负责业务数据相关；
     2、 V：视图层，顾名思义，负责视图相关，细分下来就是html+css层；
     3、 VM：V与M沟通的桥梁，负责监听M或者V的修改，是实现MVVM双向绑定的要点；
  - MVVM支持双向绑定，意思就是当M层数据进行修改时，VM层会监测到变化，并且通知V层进行相应的修改，反之修改V层则会通知M层数据进行修改，以此也实现了视图与模型层的相互解耦；

- 关系图

  ![img](https:////upload-images.jianshu.io/upload_images/3360875-0165a2d4e529f192.png?imageMogr2/auto-orient/strip|imageView2/2/w/895/format/webp)





二、Vue组件化编程

2.1 模块与组件、模块化与组件化

2.2. 组件定义与使用——(非单文件)

组件使用的基本流程：1.定义	2.注册

定义



注册：

全局注册

局部注册











2.2. 组件定义与使用——(单文件组件)



组件使用的两种流程：





二、组件化编程

# 三、使用Vue脚手架



vue-cli是vue官方提供的脚手架工具 command line interface



## 3.1使用脚手架创建模板项目

### 3.1.1 创建Vue项目

- 创建脚手架4/3的vue项目, 并运行

  ```
  npm install -g @vue/cli
  
  vue create vue-demo
  
  npm run serve
  ```

- 访问: http://localhost:8080/

### 3.1.2 项目模板结构

- vue-cli2脚手架项目结构

  ```
  gshop
  	|-- build : webpack相关的配置文件夹(基本不需要修改)
  	|-- config: webpack相关的配置文件夹(基本不需要修改)
  		|-- index.js: 指定的后台服务的端口号和静态资源文件夹
  	|-- node_modules
  	|-- src : 源码文件夹
  		|-- main.js: 应用入口js
  	|-- static: 静态资源文件夹
  	|-- .babelrc: babel的配置文件
  	|-- .editorconfig: 通过编辑器的编码/格式进行一定的配置
  	|-- .eslintignore: eslint检查忽略的配置
  	|-- .eslintrc.js: eslint检查的配置
  	|-- .gitignore: git版本管制忽略的配置
  	|-- index.html: 主页面文件
  	|-- package.json: 应用包配置文件 
  	|-- README.md: 应用描述说明的readme文件
  ```

- vue-cli3脚手架项目结构

  ```
  gshop
  	|-- node_modules
  	|-- public
         |-- index.html: 主页面文件
  	|-- src
  	   |-- main.js: 应用入口js
  	|-- babel.config.js: babel的配置文件
  	|-- vue.config.js: vue的配置文件，需要手动添加
  	|-- .gitignore: git版本管制忽略的配置
  	|-- package.json: 应用包配置文件 
  	|-- README.md: 应用描述说明的readme文件
  
  ```

  

































二、Vue组件化变成

三、使用Vue脚手架

四、Vue中的ajax

 