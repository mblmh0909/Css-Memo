
### <span id="selector">һ��selector</span>

#### ��һ����ѡ��
��ͬʱ����**�������**����ѡ������
```css
.fisrt.second{background:red}
```
������ʽ��ƥ��
```html
<div class="first second third"></div>
<div class="second first third"></div>
```
#### ����������ѡ��
������ÿ�����Զ���[]��������ƥ��
```css
a[title~="book"][href^="book"]:hover{color:red}
```
| ���� | ���� |
| ---- | ---- |
| = | һ�� |
| ~= | ���������� ����titile="book 1"��|
| \|= | ��ƥ��-ǰ��ͬ��=��en��en-�� |
| ^= | �ԡ�����ʼ  |
| $= | �ԡ������� |
| *= | ���� |

#### ��������ѡ����������ѡ����
������Ԫ��
``` css
div p{color:red}
```
ֱ����Ԫ��
``` css
div>p{color:red}
div > p {color:red}
```
����Ԫ��
``` css
div+p{color:red}
div + p {color:red}
```

#### ���ģ�α��
����α�� :link δ���� :visited �ѷ���
��̬α�� :hover ���� :active ��� :focus ����
**����**��һ��**����**

### <span id="selector">һ��selector</span>
ʿ���