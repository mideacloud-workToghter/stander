# WTC-Stander
前端样式规范
* 命名约束
    * 连接方式:
        + 使用-进行连接 eg:moduleName-typeName
    * 组合方式:
        + 模块名-模块名类型/功能
    * 嵌套:
        + 区域块命继承父/祖父-父，区域块嵌套,不建议深层嵌套
````
//举例
.grid
 .grid-title
 .grid-content
    . grid-content-lists
      . grid-content-lists td
      . grid-content-lists td button
        . grid-content-lists td button.submit
        . grid-content-lists td button.refuse
````

* sass文件的组合/分配
    * 全局样式定义（variables）:  
        + 字体大小，颜色，前缀命名定义
        + 前缀名使用mc(Midea Cloud),只有框架与模块最外层元素还有元件需要前缀名    
    * 功能函数定义（mixins）:  
    * 初始化样式（normalize）:  
        + 初始化样式避免覆盖原有系统样式
    * ICONFONT （icon-fonts）:
    * 框架定义 （layouts）
    * 模块定义 (nav,date-picker,datatable,grid,alert,switch,pages)
    * 元件定义 (button,radio,checked box,input,search,files)
