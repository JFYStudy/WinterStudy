中文版 lshort 代码用到的命令
===

## 命令和环境

```
\cmd{cmdname}
\env{envname}
```
生成命令名 \cmdname / 环境 envname，等宽字体。cmdname 参数不要带斜杠。

```
\pkg{pkgname}
\cls{clsname}
```
生成宏包和文档类的名称（无衬线字体）。

```
\marg{argument}
\marg*{argument}
\oarg{argument}
\oarg*{argument}
```
命令的必选参数/可选参数，分别为参数自动包裹大括号和中括号。不带星号的版本生成 meta 形式的 &lt;*argument*&gt;。

```
\Arg{argument}
```
独立的 meta 形式 &lt;*argument*&gt;。结合 `\marg*` 和 `\oarg*` 可排版较复杂的参数形式如 key-value。比如
> \usepackage[&lt;*key1*&gt;=&lt;*value1*&gt;,...]{&lt;*pkgname*&gt;}   
使用如下命令排版：
> `\cmd{usepackage}\oarg*{\Arg{key1}=\Arg{value1},\ldots}\marg{pkgname}`


```
\CTAN|link|
```
生成 CTAN 资源的链接。参数 link 为链接的子目录名称，如 systems/win32/miktex，macros/contrib/... 等。

## 索引

```
\cmdindex{cmdname}
\cmdindex[pkgname]{cmdname}
\envindex{envname}
\envindex[pkgname]{envname}
```
命令和环境的索引项。LaTeX 基本命令用不带可选参数的形式；宏包/文档类的命令在可选参数里指定名称。

```
\pkgindex{pkgname}
\clsindex{clsname}
```
宏包和文档类的索引项。

```
\pinyinindex{pinyin}{汉字}
```
汉字索引项，通过拼音参与排序。

## 命令环境

```
\demowidth{length}
```
用 `\rule` 命令画的一个宽度示意符号。

**command 环境** 用表格生成的一个加框的命令展示环境。多行命令在每行末尾（最后一行除外）加 \\。

**intro 环境** 每章开头的一个摘要环境。

**example 环境** 示例环境，生成源代码和示例效果。示例环境里不要涉及能分页的命令和浮动体。

**sourcecode 环境** 用于排版代码的浮动体，内部使用 `fancyvrb` 宏包的 Verbatim 环境。

