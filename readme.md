目录
*	[选择器](#一选择器)
	*	[类选择](#一类选择)
	*	[属性选择](#二属性选择)
	*	[子选择器和相邻选择器](#三子选择器和相邻选择器)
	*	[伪类](#四伪类)
*	[显示](#二显示)
	*	[行内和块](#一行内和块)
	*	[盒模型](#二盒模型)
	
### 一、选择器
***
","并列、" "子、相同属性加","
***
#### （一）类选择
可同时包含**多个连续**的类选择器。
```css
.fisrt.second{background:red}
```
以下形式都匹配
```html
<div class="first second third"></div>
<div class="second first third"></div>
```
#### （二）属性选择
可连续每个属性都用[]包裹，可匹配
```css
a[title~="book"][href^="book"]:hover{color:red}
```
| 符号 | 意义 |
| ---- | ---- |
| = | 一样 |
| ~= | 有完整单词 （如titile="book 1"）|
| \|= | 能匹配-前相同或=（en，en-） |
| ^= | 以……开始  |
| $= | 以……结束 |
| *= | 包含 |

#### （三）子选择器和相邻选择器
所有子元素
``` css
div p{color:red}
```
直接子元素
``` css
div>p{color:red}
div > p {color:red}
```
相邻元素
``` css
div+p{color:red}
div + p {color:red}
```

#### （四）伪类
链接伪类 :link 未访问 :visited 已访问
动态伪类 :hover 悬浮 :active 点击 :focus 焦点
**焦点**不一定**悬浮**

### 二、显示
#### （一）行内和块
	1.inline左至右，不独占；block上至下，独占。
	2.文字表单行内，类型表明块。
	3.内联不能设置盒模型属性。
	4.inline-block，不独占行但可设置宽度、高度、margin、padding
	5.inline-block后元素间有间隙解决方法有标签间去空格、font-size: 0等。
#### （二）盒模型
#####1.盒模型
	1.IE6宽高设置后包含了margin、border于padding。
	2.内联设置宽高及垂直方向margin无意义，垂直方向的padding会引起怪异显示禁用。
#####2.排序
	1.从上开始顺时针
	2.上下、左右
	3.上、左右、下
#####3.折叠
	1.只有block的垂直margin才有折叠，不存在padding与margin折叠
	2.float元素的margin永远不折叠
	3.如果overflow不是visible，将不与子元素折叠
	4.绝对定位不折叠。
	5.根元素不折叠。
#### （三）定位
#####1.static
z-index越大，越xi