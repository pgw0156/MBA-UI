MV-UI
======

MediaV的CSS公用模块库

## 1 文件结构：
    
### 1.1 目录结构：
        
        \reset.scss        // reset的css
        \common.scss      // 编写一些公用UI和组件UI的css
        \font.scss        // 编写一些常用板块字体的样式
        \component.scss      // 编写cmdUI的组件的样式
        
        \css\new_UI\libs  ........
        
### 1.2 模块文件：
        \css 下新建该模块名称文件夹，然后把该模块css文件放到这下面，例如:report文件夹下面的traffic\index.scss。
    
### 注：MBA项目中大部分都已经使用Sass进行书写编译，所以需要修改的是原.scss文件，然后使用Ruby的"sass base.scss base.css"指令进行编译。 

## 2 公用CSS 使用注释
### 2.1 reset.scss：
        /* 包含reset的css样式，如：清除标签默认边距、a标签的默认样式、table的重置、列表元素的样式、body内的默认字号字体 、input和textarea的默认样式等等 */
        

## 3 common.scss 使用注释
### 3.1 框架部分
### 3.2 CMD通用组件部分

#### .cmdUI-select
     注释：通用的下拉选择框
     Demo：<select class="cmdUI-select"></select>
     样例UI展示：http://
     
#### .cmdUI-btn-on
     注释：
