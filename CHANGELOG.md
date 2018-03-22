# CHANGELOG

## [v0.4.2-rc.36] 2018.03.21

* 🌟 支持在`nj`标签模板字符串语法中写`<#include>`标签。
* 🌟 `nj.createTaggedTmpl`方法支持传入`fileName`参数。

## [v0.4.2-rc.35] 2018.03.19

* 🌟 支持构建`es module`包。
* 🌟 增加`@root`和`@context`插值变量。
* 🌟 `once`扩展标签增加`name`属性。

## [v0.4.2-rc.34] 2018.03.12

* 🌟 支持构建`runtime`包。

## [v0.4.2-rc.33] 2018.03.05

* 🌟 增加表达式语法错误提示。
* 🌟 在React开发中支持插值变量的`{}`与`{{}}`语法共存。[相关文档](https://joe-sky.github.io/nornj-guide/templateSyntax/variable.html)

## [v0.4.2-rc.31] 2018.02.27

* 🌟 表达式支持编写嵌套对象字面量，如`{{ { a: { b: 1 } }.a.b }}`。
* 🌟 插值变量中任何形式的链式语法如其中有`undefined`也不会出现错误，而是返回一个空值。如`{{ a.b['c'].d }}`，a、b、c各为null时都不会报错。

## [v0.4.2-rc.28] 2018.02.13

* 🌟 为减小代码体积，使用`rollup`重新构建`dist`目录下各文件。