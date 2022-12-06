# <center>网页的基本标签</center>
## 标题标签
>\<h>\</h>



\<h1>一级标签\</h1>
\<h2>二级标签\</h2>
效果:

<h1>一级标签</h1>
<h2>二级标签</h2>

## 段落标签
>\<p>\</p>

先输入一个“p”再摁Tab，自动补全 

## 换行标签
>\<br>
## 水平线标签

>\<hr>
<hr>

## 字体样式标签
以Helloworld为例

### 粗体
>\<strong>\</strong>



效果:<strong>Helloworld</strong>

### 斜体
>\<em>\</em>



效果:<em>Helloworld</em>

## 注释和特殊符号
### 特殊符号

>**注释:\<!--注释内容-->**


>**空格: \&nbsp;**



空\&nbsp;\&nbsp;\&nbsp;\&nbsp;\&nbsp格

效果：空&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;格



>其他的特殊符号

| 符号写法 | 符号意义     |
| ----- | ---- |
| \&gt; |   &gt;   |
| \&lt; |   &lt;   |
| \&copy; |  &copy;    |

等等。

如要寻找某一特殊字符，请百度。





# <center>图像标签</center>

## 常见的图像格式
>JPG
>GIF
>PNG
>BMP(位图)

## 图像标签格式
>**\<img src="path"alt="text"title=""width="x"height="y/">**

### src(必填)
#### 相对地址
>从盘符开始写的完整路径(不推荐)

#### 绝对地址
>使用\../（回到上一级）



比如在HTML同一级文件夹下建立resources文件夹储存图片，这样使用\../便可直接进入目标文件夹

### alt（必填）
>若找不到目标图片，使用alt的内容代替

### title
>鼠标悬停的时候显示的文字

### width和height
>高度和宽度





# <center>链接标签</center>

>**\<a href="path" target=“”>"&nbsp;"\<a/>**

## href(必填)

表示要跳转到的画面
如

>href\<a href=https://www.baidu.com>\点击我解决一切问题\</a>
>href<a href="https://www.baidu.com" target="_blank" >点击我解决一切问题</a>

## target

表示窗口在哪里打开

>target="\_blank" 表示在新页面打开
>target="_self" 在自身网页打开

# <center>超链接</center>
## 页面间链接
>从一个页面链接到另一个页面

## 锚链接
>1. 需要一个标记
>2. 跳转到标记(href+后面要加上一个#)



建立标签:\<a id="我带你们打">\</a>
回到标签\<a href="#我带你们打">感恩的话\</a>

## 功能性链接
>邮件链接: \mailto:XXXXXXXX@xx.com



\<a href="mailto:xxxxxxxxx@xx.com">点击联系我</a>



>QQ链接

# <center>行内元素和块元素</center>
## 块元素
>无论内容多少，该元素独占一行
>(p、h1-h6)

## 行内元素 
>内容撑开宽度，左右都是行内元素的可以排在一行
>(a、strong、em) 

# <center>列表标签</center>
## 无序列表

>\<ul>\<li>第一个元素\</li>\<li>第二个元素\</li>\<li>第三个元素\</li>\<li>第四个元素\</li>\</ul>



效果：

<ul>
<li>第一个元素</li>
<li>第二个元素</li>
<li>第三个元素</li>
<li>第四个元素</li>
</ul>

## 有序列表
>\<ol>\<li>第一个元素\</li>\<li>第二个元素\</li>\<li>第三个元素\</li>\<li>第四个元素\</li>\</ol>



效果:

<ol>
<li>第一个元素</li>
<li>第二个元素</li>
<li>第三个元素</li>
<li>第四个元素</li>
</ol>

## 自定义列表
>\<dl>\<dt>这是列表的名字\</dt>\<dd>第一个元素\</dd>\<dd>第二个元素\</dd>\<dd>第三个元素\</dd>\<dd>第四个元素\</dd>\</dl>\
>其中**\<dt>Title\</dt>**表示**列表名称**

<dl>
<dt>这是列表的名字</dt>
<dd>第一个元素</dd>
<dd>第二个元素</dd>
<dd>第三个元素</dd>
<dd>第四个元素</dd>
</dl>

>应用：公司网站底部



# <center>表格标签</center>

><ol>
<li>单元格</li>
<li>行</li>
<li>列</li>
<li>跨行</li>
<li>跨列</li>
</ol>

## 行
>**<tr></tr>**

## 列
>**<td></td>**

>\<table >
	<tr>
		<td>1-1</td>
		<td>1-2</td>
		<td>1-3</td>
	</tr>
	<tr>
		<td>2-1</td>
		<td>2-2</td>
		<td>2-3</td>
	</tr>
	<tr>
		<td>3-1</td>
		<td>3-2</td>
		<td>3-3</td>
	</tr>
\</table>



效果：

<table >
	<tr>
		<td>1-1</td>
		<td>1-2</td>
		<td>1-3</td>
	</tr>
	<tr>
		<td>2-1</td>
		<td>2-2</td>
		<td>2-3</td>
	</tr>
	<tr>
		<td>3-1</td>
		<td>3-2</td>
		<td>3-3</td>
	</tr>
</table>

## 跨行跨列
>**使用colspan和rowspan**
>\<table >
	<tr>
		<td colspan="3">1-1</td>
	</tr>
	<tr>
		<td rowspan="2">2-1</td>
		<td>2-2</td>
		<td>2-3</td>
	</tr>
	<tr>
		<td>3-1</td>
		<td>3-2</td>
		<td>3-3</td>
	</tr>
\</table>



效果：

<table >
	<tr>
		<td colspan="3">1-1</td>
	</tr>
	<tr>
		<td rowspan="2">2-1</td>
		<td>2-2</td>
		<td>2-3</td>
	</tr>
	<tr>
		<td>3-2</td>
		<td>3-3</td>
	</tr>
</table>

# <center>媒体元素:视频和音频</center>
## 视频元素
>\<video src="" controls autoplay>\</video>
>src="资源路径"
>controls：控制条
>aotoplay：自动播放

## 音频元素

> >\<audio src="" controls autoplay>\</audio>
>src="资源路径"
>controls：控制条
>aotoplay：自动播放







# <center>页面结构分析</center>



|  元素名    |  描述    |
| ---- | ---- |
| header | 标题头部区域的位置（用于页面或页面中的一块区域） |
| footer | 标记脚部区域的内容（用于整个页面或页面的一块区域） |
| section | wed页面中的一块独立区域 |
| srticle | 独立的文章内容 |
| aside | 相关内容或应用 |
| nav | 导航类辅助内容 |


# <center>iframe内联框架</center>

>\<ifrma src="path"frameborder="0" width="300px" height="300px"name="mainFrame">\<iframe>

# <center>表单语法</center>

>\<form method="post" action="result.html">
\<p>名字：\<input name="name"type="text">\</p>
\<p>密码：\<input name="pass"type="password">\</p>
\<p>\<input type="submit"name="Button"value="提交"/>
\<input type="reset"name="Reset"value="重填"/>
\</p>
\<form>

效果：
<p>名字：<input name="name"type="text"></p>
<p>密码：<input name="pass"type="password"></p>
<p><input type="submit"name="Button"value="提交"/>
<input type="reset"name="Reset"value="重填"/>
</p>
<form>

>action:表单提交的位置
>method：提交方式
>>get方式：能在URL里看到表单信息，不安全
>>post方式：不能，安全，能传输大文件
>input type="text" name=""：文本框输入提交
>>input type="submit"提交
>>input type="reset"重填

| 属性      | 说明                                                         |
| --------- | ------------------------------------------------------------ |
| type      | 指定元素的类型。text，password，checkbox，radio，submit，reset，flie，hidden，image和button，默认为text. |
| name      | 指定表单元素的名称                                           |
| size      | 指定表单元素的初始宽度。当type为text或password时，表单元素的大小以字符为单位。对于其他类型，宽度以像素为单位 |
| maxlength | type为text或password时，输入的最大字符数                     |
| checked   | type为radio或checkbox时，指定按钮是否被选中                  |
| value     | 元素的初始值。type为radio时必须指定一个值                    |

## 单选框标签
>\<form action="result.html">
>\<p>
>\<input type="radio" value="boy" name="sex"/>男
>\<input type="radio" value="girl" name="sex"/>女
>\</p>
>\</form>
>其中name属性用来分组

效果

<form action="result.html">
<p>
性别:
<input type="radio" value="boy" name="sex"/>男
<input type="radio" value="girl" name="sex" checked/>女
</p>
</form>

## 多选框标签
>\<form action="result.html">
>\<p>
>\<input type="checkbox" value="sleep" name="hobby"/>睡觉
>\<input type="checkbox" value="code" name="hobby"/>敲代码
>\<input type="checkbox" value="girl" name="hobby"/>女生
>\<input type="checkbox" value="chat" name="hobby"/>聊天
>\</p>
>\</form>

<form action="result.html">
<p>
<input type="checkbox" value="sleep" name="hobby"/>睡觉
<input type="checkbox" value="code" name="hobby" checked/>敲代码
<input type="checkbox" value="girl" name="hobby"/>女生
<input type="checkbox" value="chat" name="hobby"/>聊天
</p>
</form>

## 按钮
>\<form action="result.html">
>\<p>
>\<input type="button" value="点击变长" name="Button"/>睡觉
>\</p>
>\</form>

<form action="result.html">
<p>
<input type="button" value="点击变长" name="Button"/>
</p>
</form>

>\<form action="result.html">
>\<p>
>\<input type="image"  src=""  name="Button"/>  
>\</p>
>\</form>



#  列表框文本域和文件域

## 下拉框
>
> \<p>
> 	\<select name="列表名称">
> 		\<option value="选项的值">中国</option>
> 		\<option value="选项的值">美国</option>
> 		\<option value="选项的值" selected>英国</option>
> 	\</select>	
> \</p>



效果：

<p>
	<select name="列表名称">
		<option value="选项的值">中国</option>
		<option value="选项的值">美国</option>
		<option value="选项的值" selected>英国</option>
	</select>	
</p>

## 文本域
>
>\<p>反馈
>	\<textarea name="textarea" cols="50"rows="10">文本内容/textarea>
>\<\p>



效果：

<p>反馈
	<textarea name="textarea" cols="50"rows="10">文本内容</textarea>
<\p>

## 文件域
>\<p>
>	\<input type=file name="files">
>
>	\<input type="button" value="上传"name="upload">
>
>\</p> 

 

效果:

<p>
	<input type=“file” name="files">
	<input type="button" value="上传"name="upload">
</p>



# 搜索框滑块和简单验证

## 邮件验证

>\<p>
>    \<input type="**email**"name="email">
>\</p>



效果:

<p>
    <input type="email"value=请输入邮箱 name="email">
</p>


## 网址验证

>\<p>
>    \<input type=“**url**"name="email">
>\</p>



效果:

<p>
    <input type="url"value="请输入网址" name="email">
</p>

## 数字验证

>\<p>
>    \<input type=“**number**"name="numberl">
>\</p>



效果:

<p>
    <input type="number" value="0000" max="100" min="0"name="number">
</p>

## 滑块

>\<p>
	\<input type="**range**" min="0" max="100" name="voice" >\step="10">
>\</p>



效果:

<p>
	<input type="range" min="0" max="100" name="voice" step="10">
</p>
## 搜索

> \<p>
>     \<input type="**search**"value="搜索内容"name="search">
> \</p>



效果：

<p>
	<input type="search"value="搜索内容"name="search">
</p>
# 表单的应用

## 隐藏域

>\<p>
>\<input type="text" value="admin" hidden>
>\</p>



效果：

<p>
<input type="text" value="admin" hidden>
</p>

## 只读

>\<p>
>\<input type="text" value="admin"**readonly**>
>\</p>
>
>> 无法更改



效果：

<p>
<input type="text" value="admin"readonly>
</p>


## 禁用

>\<form action="result.html">
>\<p>
>\性别:
>\<input type="radio" value="boy" name="sex"/>男
>\<input type="radio" value="girl" name="sex" checked >\***disabled***/>女
>\</p>
>\</form>



效果：

<form action="result.html">
<p>
性别:
<input type="radio" value="boy" name="sex"/>男
<input type="radio" value="girl" name="sex" checked disabled/>女
</p>
</form>


## 增强鼠标可用性

>\<p>
>\<**label** for="mark">你点我试试**</label>**
>\<input type="text" id="mark">
>\</p>

效果：

<p>
<label for="mark">你点我试试</label>
<input type="text" id="mark">
</p>


# 表单的初级验证

## palceholder 提示信息

>\<p>
>\<input type="text"name="username"**placeholder**="请输入用户名">
>\</p>



效果：

<p>
<input type="text"name="username"placeholder="请输入用户名">
</p>
## required  元素不能为空

>\<p>
>\<input type="text"name="username"placeholder="请输入"required>
>\</p>



效果:

<p>
<input type="text"name="username"placeholder="请输入"required>
</p>

## pattern 正则表达式

>\<p>
>\<input type="text"name="DIYmail" pattern="正则表达式">
>\</p>
>
>网站自行搜索





