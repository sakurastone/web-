# css层叠样式表

## 使用css的三种方式：

1.内联样式：标签中使用

2.内部样式：在<head>中使用<style>标签

3.外部样式：引入外部.CSS文件<link rel="stylesheet" href="">

## css三大特性：

1.继承性

2.层叠性

3.优先级

各种引入方式优先级：内联样式>内部样式-外部样式>浏览器默然样式。同等优先级情况下后面的覆盖前面的。!important无条件提升优先级。

### 导入外部样式

@import

@import url("global.css")

@import url(global.css)

@import "global.css"

## css语法

必须包含选择器和一条以上的声明

添加注释：/**/

## css选择器

1.标签选择器 div{background:red;}

2.ID选择器 #box{color:red;}

3.类选择器 .box{color:red;}

4.属性选择器:

- - `[att]` 具有att属性的元素
  - [att="val"]` 选择具有att属性且属性值等于val的E元素。
  - `[att~="val"]` 选择具有att属性且属性值为一用空格分隔的字词列表，其中一个等于val的元素。
  - `[att|="val"]` 选择具有att属性且属性值为以val开头并用连接符"-"分隔的字符串的E元素，如果属性值仅为val，也将被选择。
- 通配符 `*` 选定所有HTML标签

5. 复合选择器
6. 关系选择器

E F      后代选择器

E>F    子元素选择器

E+F	相邻兄弟选择器

## 样式取值

### 长度

**px	像素	绝对长度单位**

in	英寸	 绝对长度单位

cm	厘米	绝对长度单位

mm	毫米	绝对长度单位

q	1/4毫米	绝对长度单位

pt	点			绝对长度单位

pc	派克		绝对长度单位

**em	相对于当前对象内文本的字体尺寸	相对长度单位**

**rem	相对于根元素font-size计算值的倍数	相对长度单位**

### 颜色

1.颜色关键字：pink red

2.HEX十六进制 	#rgb	#rrggbb

3.RGB:rgb(R,G,B)三个参数

 正整数取值范围0-255	百分数取值范围0.0%-100.0%

4.RGBA	rgba(R,G,B,A)	A:Alpha透明度——取值0-1

## 背景

- background
- background-color
- background-image:url()

## 文本：

- color:字体颜色
- font-size:字体大小
- font-family:字体类型
- font-weight:字体粗细
  - normal:400
  - bold粗体700
  - bolder比继承值更重的值
  - lighter比继承值更轻的值
  - 数字取值范围：100|200|300|~|900
- font简写属性，有严格要求不建议使用
- text-transform文本转换大小写
  - none
  - capitalize每个单词第一个字母转换成大写
  - uppercase：每个单词转换成大写
  - lowercase每个单词转换成小写
- text-align水平对齐
- vertical-align垂直对齐
- text-indent文本内容缩进
- text-decoration文本装饰
- white-space是否保留文本间的空格、换行；指定文本超过边界时是否换行。

