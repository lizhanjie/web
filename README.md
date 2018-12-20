# web
## 前端框架梳理

### 写在前面

WEB前端架构是一系列工具和流程的集合，以提升前端代码的质量，并实现高效、可持续的工作流。我在参与项目开发的过程中，常常想起建筑师：夯实地基、精心布局、垒着一块一块的砖头、抹着一铲子一铲子的泥土。

WEB前端经历着风起雨涌，日新月异的变化。从静态走向动态，从一端走向多端，从前台走向全端。

`记得大神阮一峰说过：未来只有两种软件端工程师和云工程师，端工程师就包括手机端、PC端等，可见WEB端的不可或缺行。`


### 架构图

图片: https://uploader.shimo.im/f/NTPP6YheTkYA7NiP.jpg

### 前端的那些事：

从1994年，这一年10月网景推出了第一版的Navigator，这一边Tim Berners-Lee创建了W3C组织，这一年Tim发布了CSS，但是缺少一种语言实现用户或者浏览器可以与网页互动，1995年Brendan Eich创造了JavaScript，一种既想Java又不是Java的弱类型语言，由于涉及的比较匆忙，没有考虑太多的细节，所以造成了写出来的程序混乱不堪，也没有想到未来会成为互联网第一大语言。

总的来说，他的设计思路是这样的：
  （1）借鉴C语言的基本语法；
  （2）借鉴Java语言的数据类型和内存管理；
  （3）借鉴Scheme语言，将函数提升到"第一等公民"（first class）的地位；
  （4）借鉴Self语言，使用基于原型（prototype）的继承机制。


#### WEB前后端

WEB前端主要包括Javacript，Html，Css三门基础语言。
语法：主要是用的ES6，ES7，SASS，LESS，JADE等语法；
打包器：Webpack等；
构建工具：Gulp、Grunt等；
模板引擎：Juicer、doT、Nunjucks等；
DOM操作库：Jquery，Zepto等；
框架：Vue、React、Angular等；
WEB服务端主要是Node平台。
语法：主要是用的ES6，ES7语法;
I/O：非阻塞；
驱动：事件驱动；
线程：单线程；
宿主：V8虚拟机；
框架：KOA、EXPRESS

#### 开发规范

W3C标准，用来规范结构（Structure）、表现（Presentation）和行为（Behavior）。
推荐配置：
Javascript：Eslint（standard）
Html：W3C标准（语义化）
Css：W3C标准（简洁化）

#### 工具

脚手架工具（generator），统一组件的构建方式
framework，对EGG一些请求和认证等的封装
代码仓库（git），管理代码仓库
辅助工具（f2e），对上传，EGG的包等进行构建
npm脚本，对一些日常提交，起动环境等进行封装
云凤蝶，可配置的静态模板引擎
python
...

#### 组件

`站在巨人的肩上，我们能走的更高`

好的组件能加快项目构建速度，比如认为比较优秀的组件库如：Ant Design、Element UI、React系列等。
目前WEB前端组已经沉淀出很多高服用的组件，如Stroage、DataPicker系列、AppBridge、ComImg等等，已应用到各个业务线，至少可以提高5-7倍的人效，同时还沉淀出相关的技术文档，降低了后期的维护成本。

#### 技术选型

技术选型的重要性，就像高考报志愿，选的好，不仅可以降低维护成本，还可以加快构建速度！一般得现在目前前端流行的都是混合型构建方案，没有最好的，只有更适合的。
比如：
`react + redux + es6 + webapck(适合交互比较强的PC站)；
vue + vuex + es6 + webpack(适合MOBILE站) ;
jucer + zepto + es6 + webpack(适合活动等静态站)；
node + webpack + vue + vuex + es6(适合项目比较大的站点)；
...`


#### 兼容策略

在各大浏览器厂商的发展过程中，他们其实对web的标准都有不同的实现，因为实现的标准的不同，所以会有兼容性的产生。通俗的说，就是对于web标准，有些浏览器支持，有些浏览器不支持。也是前端最头痛的事情...
每个项目，乃至每个公司都自己的一套HACK手段，在项目中加入很多好的plugins。CSS兼容推荐用postcss-loader插件，JS兼容推荐babel-loader插件等。

### 一个例子
