### һ��selector
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
###����������ѡ��
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
