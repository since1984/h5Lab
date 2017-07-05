# jquery 整体框架

> 网上的，感觉有点老，先备着

- 变量，常用正则初始化
- 工具方法 $.fn
- $.ready()
- 复杂选择器Sizzle
- 回调对象：对函数的统一管理$.Callback()
- 延迟对象：对异步的统一管理$.Deferred()
- 浏览器功能性检测$.support
- 数据储存$.data
- 队列方法：执行顺序的管理queue() | dequeue()
- 对元素属性的操作attr(),prop(),val(),addClass()等
- 事件操作的相关方法on(),trigger()
- DOM操作
- 样式操作css()
- Ajax()
- 动画animate()
- 位置和尺寸offset()
- 模块化
- window.jQuery = window.$ = jQuery;

# Sizzle

选择器表达式

- 块表达式
  - 简单表达式
    - id
    - class
    - tag
  - 属性表达式
  - 伪类表达式
    - 位置伪类
    - 子元素伪类
    - 内容伪类
    - 可见伪类
    - 表单伪类
- 块间关系
  - “>”父子关系
  - " " 祖先后代关系
  - "+"紧邻兄弟元素
  - "~"之后的所有兄弟元素

