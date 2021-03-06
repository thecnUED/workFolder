# 招聘规划

## 项目前端当前面对的问题

### Javascript

1. 代码规范，开发规范和前端工作流的重建
2. 前端架构

    1. View层

        1. backbone.layoutManage插件的运用不得当，导致dom渲染顺序无法保证，例如：

            afterRender方法不总是在render后触发
            先渲染大框架再渲染小部件的方式导致无法在代码内获取到dom的样式信息：在afterRender方法内获取this.$el.height总是0，因为该节点还未插入dom树

        2. view的搭建数据共享：main->box->item->xxx->... 数据传递通过new时的构造函数传给下一个view的init方法，导致嵌套关系太深，信息容易在其中一节丢失

    2. Model层

        1. 类继承方式不完善
        2. 没有错误处理机制
        3. 没有最大限度地利用事件驱动方法与view进行协作
 
3. 前后台数据通讯

    当前复写了backbone.sync方法，复写了model, collection的保存/删除/查询方法

4. 单元测试系统的构建

### CSS

在公共部分，当前已经有了一套解决方案：[ChopperUI](https://github.com/chopper-UI)。
目前阶段需要思考的问题是：各自block的样式与组件库如何协同工作？例如：
新的功能是建立一个表单layout，我们可以使用form.css轻易完成这个功能，但是每一个layout都会有其特征性的表现，这时候我们如何应对？class声明规则如何？

## 招聘方向

针对项目当前面对的问题，招聘应以重JS技能为主，强调工程能力。
要求为：

1. 一年以上的前端领域开发经验，能独立完成前端开发工作；
2. 热衷学习与自我修炼，喜欢阅读技术文档和书籍；
3. 熟练运用HTML/CSS/Javascript等前端技术，能写出符合W3C标准、兼容主流浏览器的代码；
4. 熟练掌握至少一种JS框架或者对JS语言掌握较好；
5. 有面向对象开发经验，对设计模式有一定了解；

## 招聘规划

1. 招聘途径

    在51job发布职位或主动联系符合要求的程序员，约定时间进行面试。

2. [面试流程](https://github.com/thecnUED/workFolder/blob/master/interview/%E9%9D%A2%E8%AF%95%E6%B5%81%E7%A8%8B.md)

