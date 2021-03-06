# 一、缩进
采用”\&ensp;“或者“\&emsp;”即可，前者代表一个半角空格，后者代表两个半角空格，如果需要汉字段首行缩进，四个前者或者两个后者即可。
# 二、字体
- 加粗<br />
要加粗的文字左右分别用两个*号包起来
- 斜体<br />
要倾斜的文字左右分别用一个*号包起来
- 斜体加粗<br />
要倾斜和加粗的文字左右分别用三个*号包起来
- 删除线<br />
要加删除线的文字左右分别用两个~~号包起来
# 三、引用
在引用的文字前加>即可。引用也可以嵌套，如加两个>>三个>>>
n个...
貌似可以一直加下去，但没神马卵用
# 四、分割线
三个或者三个以上的 - 或者 * 都可以<br />
# 五、图片
![图片alt](图片地址 ''图片title'')
#### 不同编辑器中似乎显示的方式不同
    ![]("https://github.com/2500664779/OperationSystem/raw/master/studyReview/pictures/1.3.jpg")
    ![](pictures\1.3.jpg)
分别为github和vscode编辑器中查看的方式
# 六、超链接
[超链接名][超链接地址]
# 七、列表
## 无序列表
语法：无序列表用 - + * 任何一种都可以  
## 有序列表
注意，数字和内容之间要有空格
1. 列表内容
2. 列表内容
3. 列表内容
## 列表嵌套
## 上一级和下一级之间敲三个空格即可
# 八、表格
语法：
表头|表头|表头
---|:--:|---:
内容|内容|内容
内容|内容|内容

第二行分割表头和内容。
- 有一个就行，为了对齐，多加了几个<br />
文字默认居左<br />-两边加：表示文字居中-右边加：表示文字居右
注：原生的语法两边都要用 | 包起来。此处省略
# 九、代码
语法：
单行代码：代码之间分别用一个反引号包起来
代码块：代码之间分别用三个反引号包起来，且两边的反引号单独占一行
```
this is coding area;
<code>code here</code>
<pre>code here</pre>
```

&emsp;&emsp;同各种程序语言相关的写作或是标签语言原始码通常会有已经排版好的代码块，通常这些代码块我们并不希望它以一般段落的方式去排版，而是照原来的样子显示，Markdown 会用 **\<pre>**和**\<code>** 标签来把代码区块包起来。
Markdown建立代码块的方法：只要在行最前面简单地缩进 4 个空格或是 1 个制表符就可以，一个代码区块会一直持续到没有缩进的那一行。


# 十、流程图
```
```flow
st=>start: 开始 
op=>operation: My Operation
cond=>condition: Yes or No?
e=>end
st->op->cond
cond(yes)->e
cond(no)->op
&```  
```

    \[fjdskalfjdsaklfja \] 可以居中
\[fjdskalfjdsaklfja \]