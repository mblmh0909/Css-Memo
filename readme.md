
### <span id="selector">一、selector</span>

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

### <span id="selector">一、selector</span>
士大夫