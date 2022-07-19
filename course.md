# 1. 标题

使用=展示一级标题
=
使用-展示二级标题
-
也可以使用#展示1-6级标题
# 一级标题
## 二级标题
# 2. 字体
*斜体字体*
_斜体字体_
**粗体字体**
__粗体字体__
***粗斜体字体***
___粗斜体字体___
## 分隔线
可以在一行中用三个*或-或_来建立一个分隔线。
***
watson

---
handsome
___
## 删除线
文字两端加~~即可
~~删除~~
## 下划线
<u>带下划线文本<u>
## 脚注
创建脚注格式类似这样 [^test]
[^test]:我是脚注格式。
# 3. 列表
无序列表 使用*、+、-作为标记，记得加空格。
* 第一项
* 第二项
* 第三项

有序列表 使用数字并加上.号来表示。

1. 第一项
2. 第二项

列表嵌套 在子列表的选项前面添加四个空格。
* 第一项
    * first
    * second
    * third
* 第二项
    - forth
    - fifth
    - sixth

# 4. 区块
区块引用 在段落开头使用 > 符号跟一个空格。
> 区块引用

blablabla
> Markdown

区块嵌套 一个 > 是最外层，两个 > 是一层嵌套。
> 第一层
>> 第二层
>>> 第三层

区块中使用列表
> 区块
> 1. 列表一
> 2. 列表二
>     - 子列表一
>     - 子列表二

列表中使用区块
* 第一项
    > 区块
* 第二项
# 5. 代码
如果是段落上的一个函数或片段代码可以用反引号包起来（`）。

`printf()`函数

代码区块  使用4个空格或者一个制表符。

    int function()
    {
        code;
        ...
        return 0;
    }

也可以用```包裹一段代码 并指定一种语言

```C
int function()
{
    printf("hello world!");
    return 0;
}
```

# 6. 链接
链接使用方法：
[链接名称](链接地址)
或者
<链接地址>

这是[百度链接](www.baidu.com)

高级链接  通过变量设置链接，在末尾为变量赋值。
这是[百度链接][1]
这是[谷歌链接][2]

[1]: www.baidu.com
[2]: www.google.com

# 7. 图片
![alt 属性文本](图片地址)
![alt 属性文本](图片地址 "可选标题")
- 开头一个感叹号
- 然后中括号里放上图片的替代文字
- 最后小括号放上图片的网址 可选标题

![猫咪](https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fwww.2008php.com%2F2014_Website_appreciate%2F2014-02-15%2F20140215220958.jpg&refer=http%3A%2F%2Fwww.2008php.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1660838586&t=ed90c99392584f7b1fae1fecf4f4cb04 "小猫咪")

也可以像网址一样使用变量。
![猫咪][3]

[3]: https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fwww.2008php.com%2F2014_Website_appreciate%2F2014-02-15%2F20140215220958.jpg&refer=http%3A%2F%2Fwww.2008php.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1660838586&t=ed90c99392584f7b1fae1fecf4f4cb04

MD还没有办法指定图片的高度和宽度，如果需要可以使用img标签。
<img src="https://gimg2.baidu.com/image_search/src=http%3A%2F%2Fwww.2008php.com%2F2014_Website_appreciate%2F2014-02-15%2F20140215220958.jpg&refer=http%3A%2F%2Fwww.2008php.com&app=2002&size=f9999,10000&q=a80&n=0&g=0n&fmt=auto?sec=1660838586&t=ed90c99392584f7b1fae1fecf4f4cb04" width="50%">

# 8. 表格
使用|来分隔不同的单元格，使用-来分隔表头和其他行。

价格 | 数量
- | -
10 | 10
20 | 20
30 | 30

对齐方式
* -: 设置内容和标题右对齐
* :- 设置内容和标题左对齐
* :-: 居中对齐

| 左对齐    |    居中对齐    |    右对齐 |
|  :-  |   :---: |   --: |
| 队列一 | 队列二 | 队列三 |
| 队列四 | 队列五 | 队列六 |

# 9. 高级技巧
支持HTML元素
目前支持的HTML元素有：<kbd><b><i><em><sup><sub><br>等。

使用<kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd>重启电脑。

转义  加上反斜杠符正常显示字符 如\*\*粗文本\*\*

公式  
* $...$会在行内显示
* $$...$$会在块内显示

$$
\begin{Bmatrix}
   a & b \\
   c & d
\end{Bmatrix}
$$
$$
\begin{CD}
   A @>a>> B \\
@VbVV @AAcA \\
   C @= D
\end{CD}
$$

END