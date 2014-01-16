MV-UI
======

MediaV的CSS公用模块库

## 技术框架：MBA项目中大部分都已经使用Sass+Compass进行编写编译和构建的，每次修改的需要是原.scss文件。(compass里面的mixin.sass的一些“函数”还是能节约一部分代码的，另外还有css3的部分) 

## 1 文件结构：
    
### 1.1 公用scss文件概览：
        /* 以下每个.scss文件皆单独编写，可以考虑完成后放在静态域名下？ */
        /reset.scss       // reset的css
        
        /common.scss        // 定义一些比较常用的基本样式，分类有：框模型、定位、对齐、常用尺寸等，如：.p-r {position:relative;}
        
        /font.scss        // 一些常用板块字体的样式，按照光宇出的样式编写，另外还有一些常用的字体字号行高，如：.font-tips {font-size:12px; color:#ca1a00; }  .f-12 {font-size:12px;}
        /icons.scss       // 各种小icon的集合(还有hover状态的)，小icons都用css sprite合并成一张图片，如：.icon-help {}
        
        /component-common.scss   // 根据潘爷吴氏控件库的通用控件模块进行编写 (适当调整和选取)
        /component-content.scss  // 根据潘爷吴氏控件库的内容展示控件模块进行编写
        /component-base.scss     // 根据潘爷吴氏控件库的基础控件模块进行编写
        
        /* 这个大概把基础的公用组件涵括了，编译到一个.css文件里面 */
        /mvui.scss      // 把需要的子scss文件导入进来进行编译，合并成一个文件mvui.css，具体代码：@import "reset.scss"; @import "font.scss";
------------------------------------------------------—我是分界线--------------------------------------------------------        
        /* 下面是具体到每个系统层面的东西了 */
        
        theme-dmp.css，theme-atd.css   // 相当于一个相当于皮肤的css文件包括对上面基础css文件的样式进行修改补充，主要是每套系统的个性化的地方，例如：.nav { background:red; border-color:grey; }
        common-dmp.css，common-atd.css // 该系统的一些独有的公用样式
        
        /各个JS功能组件库.css，如：radio.css，tab.css
        /各个JS业务组件库.css，如：table-mba.css，dateSelector.css
         
### 1.2 模块文件：
        /* css 根据各模块需要下新建该模块名称文件夹，然后把该模块css文件放到这下面，例如:report文件夹下面的traffic\index.css */
        

## 2 公用CSS 使用注释
### 2.1 reset.scss：
        /* 包含reset的css样式，如：清除标签默认边距、a标签及其伪类的默认样式、table的重置、列表元素的样式、body内的默认字号字体 、input和textarea等的默认样式等等 */
        可以直接使用compass里面的内嵌reset样式，@import "compass/reset"，另外还需要一些全局变量
        

## 3 潘爷吴氏css 使用注释
### 3.1 mv通用控件模块(component-common.scss)
#### .mvui-modal
     注释：传说中的蒙太层
     Code Demo：
     <div class="mvui-modal">
        <div class="title"><span class="icon-straight"></span>点我获取代码</div>
        <div class="content">今天看到扮XXX是结识美女的好办法</div>
     </div>
     样例UI展示：http://xxxxxx

### 3.2 mv内容展示控件模块(component-content.scss)    
#### .mvui-rank
     注释：据说这个是排名的编号
     Code Demo：
     <div class="mvui-rank">
        <span class="numType1">1.</span>
        <span class="numType2">2.</span>
        <span class="numType3">3.</span>
     </div>
     样例UI展示：http://xxxxxxxx
     
### 3.3 mv基础控件模块(component-base.scss.scss)    
#### .mvui-select
     注释：那个普通的下拉选择框
     Code Demo：
     <div class="mvui-select">
        <option value="kfc">圣代</span>
        <option class="mac">新地</span>
     </div>
     样例UI展示：http://xxxxxxxx
     
