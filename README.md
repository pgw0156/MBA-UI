MV-UI
======

MediaV的CSS公用模块库

### 注：MBA项目中大部分都已经使用Sass+Compass进行编写编译和构建的，每次修改的需要是原.scss文件。(compass里面的mixin.sass的一些“函数”还是能节约一部分代码的) 

## 1 文件结构：
    
### 1.1 公用scss文件概览：
         /* 单独编写，可以考虑完成后放在静态域名下 */
        \reset.scss       // reset的css,在compass下
        \font.scss        // 一些常用板块字体的样式，按照光宇出的样式编写，如：.font-tips {font-size:12px; color:#ca1a00; }
        \
        \component.scss   // 编写cmdUI的组件的样式
        
        \mvui.scss        // 把需要的子scss文件导入进来进行编译，合并成一个文件，如：@import "reset.scss";@import "font.scss";
        
        
### 1.2 模块文件：
        \css 下新建该模块名称文件夹，然后把该模块css文件放到这下面，例如:report文件夹下面的traffic\index.scss。
    


## 2 公用CSS 使用注释
### 2.1 reset.scss：
        /* 包含reset的css样式，如：清除标签默认边距、a标签的默认样式、table的重置、列表元素的样式、body内的默认字号字体 、input和textarea的默认样式等等 */
        可以直接使用compass里面的内嵌reset样式，@import "compass/reset"，另外还需要一些全局变量
        

## 3 common.scss 使用注释
### 3.1 框架部分
### 3.2 mv通用组件部分

#### .mvui-select
     注释：通用的下拉选择框
     Demo：<select class="mvui-select"></select>
     样例UI展示：http://
     
#### .mvui-radio
     注释：
