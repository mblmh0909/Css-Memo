Ŀ¼
*	[ѡ����](#һѡ����)
	*	[��ѡ��](#һ��ѡ��)
	*	[����ѡ��](#������ѡ��)
	*	[��ѡ����������ѡ����](#����ѡ����������ѡ����)
	*	[α��](#��α��)
*	[��ʾ](#����ʾ)
	*	[���ںͿ�](#һ���ںͿ�)
	*	[��ģ��](#����ģ��)
	*	[��λ](#����λ)
	*	[](#)
	
### һ��ѡ����
***
","���С�" "�ӡ���ͬ���Լ�","
***
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

### ������ʾ
#### ��һ������
#####1.display
	1.inline�����ң�����ռ��block�����£���ռ��
	2.���ֱ����ڣ����ͱ����顣
	3.�����������ú�ģ�����ԡ�
	4.inline-block������ռ�е������ÿ�ȡ��߶ȡ�margin��padding
	5.inline-block��Ԫ�ؼ��м�϶��������б�ǩ��ȥ�ո�font-size: 0�ȡ�
#####2.float
	1.������󸡶��ˣ�������ʾЧ��Ϊblock��CSS3���ó�run-i���ⲻ�䡣
	2.**������ֱmargin�����۵�**
	3.clear����������ڵĸ�����ֵ����Ϊleft��right��both��
#### ��������ģ��
#####1.��ģ��
	1.IE6������ú������margin��border��padding��
	2.�������ÿ�߼���ֱ����margin�����壬��ֱ�����padding�����������ʾ���á�
#####2.����
	1.���Ͽ�ʼ˳ʱ��
	2.���¡�����
	3.�ϡ����ҡ���
#####3.�۵�
	1.ֻ��block�Ĵ�ֱmargin�����۵���������padding��margin�۵�
	2.floatԪ�ص�margin��Զ���۵�
	3.���overflow����visible����������Ԫ���۵�
	4.���Զ�λ���۵���
	5.��Ԫ�ز��۵���
#### ��������λ
#####λ��
	1.static��relative��absolute��fixed��
	2.relative�����**������λ**ƫ��
	3.absolute�����**��һ������λԪ��**ƫ��
	4.fixed�����**����**ƫ��
#####��ֱ
	z-indexͬ�㼶��z-index�Ż�ȴ�С��
	���´��뾡���ڲ�div��z-index aaa�����bbb�㵫�����z-index bbb�����aaa�㣬������bbb�㸲��aaa��
```html
<div style="position:absolute;z-index:3"><div style="position:absolute;z-index:1000;background:red">aaa</div></div>
<div style="position:absolute;z-index:30"><div style="position:absolute;z-index:10;background:blue">bbb</div></div>
```