MBA-UI
======

MBA系统的UI规范和公用模块

## 1 文件结构：
    
### 1.1 基础文件：
        \css\new_UI\base.css        // 基础base的css
        \css\new_UI\common.css      // 编写一些公用UI和组件UI的css
        \css\new_UI\libs  ........
### 1.2 模块文件：
        \css 下新建该模块名称文件夹，然后把该模块css文件放到这下面，例如:report文件夹下面的traffic\index.scss。
    
### 注：MBA项目中大部分都已经使用Sass进行书写编译，所以需要修改的是原.scss文件，然后使用Ruby的"sass base.scss base.css"指令进行编译。 

## 2 base.css 使用注释


## 3 common.scss 使用注释
### 3.1 框架部分
### 3.2 CMD通用组件部分

#### .cmdUI-select
     注释：通用的下拉选择框
     Demo：<select class="cmdUI-select"></select>
     样例UI展示：http://
     
