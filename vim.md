
vim ntoe
=========

# vim
## use ikjl to move!!! ri le!!!
	noremap h i
	noremap i k
	noremap k j
	noremap j h

	noremap H I
	noremap I K
	noremap K J
	noremap J H

## 文件
:e打开文件
:s替换
:h帮助
:w,q,wq,q! 存盘, 退出等
## 移动
hjkl
w 向后单词头, b 向前单词头, e 单词尾
( ) 句首句尾
{ } 段首段尾   [[ ]] 文件首尾
^ $ 行首尾
- + 前一行后一行首 
zt, zb, zz把当前行至于屏幕顶部, 底部, 中间
## 查找
/ ? 匹配, 反向
n N 下一个, 反向  :noh关闭高量
%括号匹配
#反向查找
\* 直接搜索游标处单词
f F行内字符查找/反向查找
t T下一个字符前一个位置

## 选择

v 标记 V标记行, Ctrl V 块操作
'< '> 引用v的内容
vi 内部
va 外部
vit tag内部
vi" 引号内部
viw 选择词
## 操作
. 重复指令  u 撤销 ctrl - R 重做
i s a o 进入编辑模式   i当前位置, s删除当前, a下一位置, o下一行, ISA分别是首, 删行, 尾, O是上一行
r 替换, R连续替换, 实际上就是替换模式
p 粘贴
接范围的指令, 行数, 光标位置 web{}()^$-+等
d 删除指令, dw, db  D删除至行末
< > 缩进
y 复制  Y复制行
c 修改且进入编辑模式, cc 修改当前行, C修改至行末, 即删除至行末尾并且进入insert模式

dw、diw 刪除游標所在的那一個字(word)
cw、ciw 刪除游標所在的一個字(word)並直接進入insert mode
x X删除, 退格
~ 转换大小写
## 好用命令
= 格式整理，gg=G 整份文件格式自動整理

:tabe 開新tab
gt 切換至下一個tab；gT 切換至上一個tab。(在我的vimrc裡有分別對應到F7跟F8鍵)
:new 新增水平分割視窗；:vnew 新增垂直分割視窗。

q: 命令行窗口


## 窗口
:n
:N

:ls 查看当前打开的buffer（文件）
:b num 切换文件（其中num为buffer list中的编号）
":bn" -- next buffer in the buffer list 

":bp" -- previous buffer in the buffer list
":b#" -- previous buffer you was in 

ctrl tab切换窗口

:split vertical split 
:close 

:only
:new 

:enew
:qall
:wall :ball

## tab
:tabedit thatfile
:tab split tabonlytab help gt在任何打开窗口的 Ex 命令前面，你都可以放上 ":tab"ctrl pageup pagedown 切换tab

## diff
vimdiff main.c~ main.c  
:vertical diffsplit main.c
:diffupdate(手动更新)  
:dp(用左边的文件做参考复制修改)  

:do(用右边的文件作参考复制修改) 
##其他
ctrl f b 翻页
ctrl E Y 滚屏
!外部过滤器
  
`
'
;
,
m
q Q
@
&
z Z
  
## 其他
==================
{hel*lo}
比如我们有如上的例子，*表示光标停留的位置，如果我们使用vi}, 就可以选择hello，如果使用va},那么选择的就是{hello}
=======
列操作C-V
如果需要在后面追加，就按A，然后输入要插入的内容，接下来按ESC就可以看到添加的内容了。如果需要在某一列添加，就使用I。这样如果我们需要在行尾加注释的话，那么我们就可以这样来操作了

<ESC> 0 <C-Q> 5 j I //<ESC>
如果需要删除行头的注释，可以使用如下的快捷键

<ESC>0<C-Q>l5jx<ESC>
## 92上vim配置错误信息
	>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

	处理 /public/luhr/.vim/plugin/acp.vim 时发生错误:
	第   11 行:
	AutoComplPop does not support this version of vim (700).
	处理 /public/luhr/.vim/plugin/tagbar.vim 时发生错误:
	第 1138 行:
	E475: 无效的参数: 141
	第 1159 行:
	E475: 无效的参数: 144
	第 1176 行:
	E475: 无效的参数: 142
	第 1206 行:
	E475: 无效的参数: 143
	第 1211 行:
	E475: 无效的参数: 144
	第 1217 行:
	E475: 无效的参数: 148
	第 1222 行:
	E475: 无效的参数: 149
	第 1227 行:
	E475: 无效的参数: 150
	第 1232 行:
	E475: 无效的参数: 151
		请按 ENTER 或其它命令继续