MyNote&Config of Sublime Text Editor
Sublime Text - An Excellent Replacement of GNU Emacs.


# keyboard binding
Only have ctrl+x prefix, there is no ctrl+c and other prefix.
The only exception is "ctrl+x, ctrl+x": "cut". 
## Single Keys
括号里是重复兼容emacs的部分按键.
"/" 隔开的前面是ctrl, 后面是alt, shift和ctrl-x只作为ctrl辅助, 没有ctrl+c前缀, ctrl+c只有复制含义.
alt一般和一些对应操作或者文件操作联系起来. 
	添加一行
	   
	f2   bookmark 下一个, C设置, S上一个/选择所有 bookmark
	f3   查找下一个, C查找当前单词, S上一个/选择所有
	f4   
	f7   build
	f9   行排序
	f10  markdown preview
	f11  全屏, 专注模式
	f12  在浏览器中查看
	1-9  切换组/切换tab
	q    录制宏, 播放宏/进入vi模式/ ctrl+alt+q 
	w    删除, 关闭/关闭
	e    行尾/翻页
	r    反向查找/
	t    交换, tag, 重新打开文/
	y    (黏贴)/(黏贴环)
	u    大写/小写
	i    上/段落移动
	o    del, **扩展选区到scope**/单词删除
	p    goto everthing/命令palette    //呼出各种palette
	[    缩进, folding/
	]    缩进, folding/
	\    
	a    行首, 全选C-xa/翻页
	s    正向查找/存盘  
	d    选择单词, 多选相关, 复制行/
	f    查找/goto everthing
	g    取消/goto line, tag, methord //其实只需要goto everthing就够了
	h    退格/单词退格
	j    左/单词左
	k    下/段落下
	l    右/单词
	;    注释/块注释
	'    切换到sidebar/    
	z    撤销,重做/重复
	x    剪切,前缀/
	c    复制/
	v    黏贴/黏贴环
	b    选择段落/goto open files
	n    删除行, 选择行/删到段       //不设置kill整行
	m    选择行, 选择到缩进/                   
	,    /翻页
	.    /翻页      //close tag
	/    撤销,重做/自动补全

ctrl+,/.设置不能, 原因不明, 可能是因为搜狗输入法

## Navigating

	| ctrl+ikjl                     | move           |
	| alt+il                        | move word      |
	| alt+ik                        | move paragraph |
	| ----------------------------- | -------------- |
	| alt+,. or pageup, pagedown    | move page      |
	| ctrl+a,e or home, end         | line home, end |
	| alt+a/e                       | 翻页             |
	| ctrl+home,end or alt+shift+,. | file home&end  |
	| ctrl+9/0                      | 跳转至对应括号        |
	| ctrl+alt+0                    | 跳转至sidebar     |

"overlay_scroll_bars": "enabled" 隐藏scrollbar
Adding shift will select. 

注意ctrl+,.有意义
## Editing

	| c-c or m-w                         | copy                  |
	| c-x c-x                            | cut                   |
	| c-vy  ,c-s-v                       | paste, 黏贴并自动缩进        |
	| m-vy                               | paste circle          |
	| ctrl+shift+d                       | 复制当前行                 |
	| ctrl+xw                            | cut到标记                |
	| alt+w                              | copy到标记               |
	| ctrl+w                             | 退格删单词                 |
	| ------------------                 | --------              |
	| ctrl+/, u, z,                      | undo                  |
	| ctrl+shift+ /, u, z,               | redo                  |
	| --------                           |                       |
	| ctrl/alt+;                         | comment               |
	| ctrl+shift+;                       | block comment         |
	| --------------                     |                       |
	| ctrl+w                             | 退格删单词                 |
	| ctrl+h/o                           | 退格/删除                 |
	| ctrl+shift+h                       | 向前删除到行首               |
	| ctrl+m                             | 向后删除到行尾, 进入killring   |
	| ------------   f, g : goto         |                       |
	| ctrl+shift+f                       | project 查找替换          |
	| alt+f, ctrl+alt+f, ctrl+xf, ctrl+p | 打开文件, goto everything |
	| ctrl+xb, alt+b                     | 到open file            |
	| alt+g                              | 到行:                   |
	| ctrl+alt+g                         | 到tag@                 |
	| ctrl+shift+p,alt+p                 | 到命令                   |
	| ctrl+alt+p                         | 到project              |
	| ctrl+x,b                           | next view             |
	| ----------                         |                       |
	| ctrl+s/r, f                        | 查找                    |
	| ctrl+alt+r                         | 替换                    |
	| ctrl+shift+f                       | project 查找替换          |
	| f3, shift+f3                       | 下一个, 上一个, 查找词或者当前词    |
	| ctrl+d, ctrl+xd 跳过当前               | 扩展选择当前词               |
	| alt+f3                             | 选择所有当前词               |
	| ----------                         |                       |
	| alt+/                              | 补全                    |
	| ctrl+shift+up,down                 | 上下移动行或者多行             |
	| -----------------                  |                       |
	| f6                                 | 拼写检查toggle            |
	| ctrl+f6, ctrl+shift+f6             | 下一个, 上一个拼写检查          |
	| f9 , ctrl+f9(case sensitive)       | 行排序                   |
	| ---------                          |                       |
	| ctrl+alt+u/l  or ctrl+xu/xl        | 改成大写, 小写              |



//edit 菜单里面还有排列行, 排列选区功能
//搜狗输入法快捷键 ctrl+shift+q 表情, +e 英文输入法
## Selecting

	| ctrl+space                  | 标记                |
	| shift+定位                    | 选择                |
	| -------------               | ---------         |
	| ctrl+n 一般都要shift, 这里是简化     | 扩展到行              |
	| ctrl+shift+m,9,0,o,n        | 扩展到行,括号,scope, 缩进 |
	| b                           | 扩展到段落             |
	| ctrl+x, ctrl+a or ctrl+x, h | 全选                |
	| ctrl+d                      | 扩展选择当前词           |





### Misc, Window, Sidebar

	| ctrl+x,u              | 转换为utf8          |
	| --------              |                  |
	| ctrl+x, 1, 2, 3       | 切换窗口显示           |
	| alt+shift+数字          | 切换窗口显示           |
	| ------------          |                  |
	| ctrl+0                | 切换到侧边栏           |
	| ctrl+x,ctrl+z         | 切换侧边栏显示          |
	| ---------------       |                  |
	| view-->keymap manager | 管理keymap冲突       |
	| ctrl+shift+t          | reopen last file |
	| ctrl+alt+t            | find todos       |


## Indention, Folding, Table
### 缩进和tab

	| tab           | 自动缩进               |
	| shift+tab     | 在行首是倒回缩进, 行内是普通tab |
	| ctrl+[]       | 调整缩进               |
	| ctrl+shift+,. | 调整缩进               |
	| ----------    |                    |
	| alt+q         | wrap lines         |

### Folding

	| ctrl+shift+[] | fold, unfold |

### MD模式
MD语法 [https://gitcafe.com/riku/Markdown-Syntax-CN/blob/master/basics.]
showdown.js [http://softwaremaniacs.org/playground/showdown-highlight/]
strapdown js [http://strapdownjs.com/]
highlight.js [http://johannburkard.de/blog/programming/javascript/highlight-javascript-text-higlighting-jquery-plugin.html]

markdownediting 插件 编辑辅助
原背景颜色<string>#ECECEC</string>
markdownpreview 插件 生成辅助

	| tab       | 收起展开当前项目 |
	| shift+tab | 收起, 展开所有 |

### Table
//table editor

	 { "keys": ["ctrl+alt+j"], "command": "table_editor_join_lines", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "(\\|)|(\\+)", "match_all": true }
	        ]
	    },
	{ "keys": ["ctrl+x","-"], "command": "table_editor_insert_single_hline", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "$", "match_all": true }
	        ]
	    },
	    { "keys": ["ctrl+x","="], "command": "table_editor_insert_double_hline", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "$", "match_all": true }
	        ]
	    },
	    { "keys": ["ctrl+x","enter"], "command": "table_editor_hline_and_move", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "$", "match_all": true }
	        ]
	    },
	    { "keys": ["ctrl+x","|"], "command": "table_editor_csv_to_table", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true }
	        ]
	    },
	### Gist
	  //gist
	  { "keys": ["ctrl+x", "ctrl+i"], "command": "gist" },
	  { "keys": ["ctrl+x", "ctrl+p"], "command": "gist_private" },
	  { "keys": ["ctrl+x", "ctrl+s"], "command": "gist_update_file" },
	  { "keys": ["ctrl+x", "ctrl+o"], "command": "gist_list" },
	  { "keys": ["ctrl+x", "ctrl+["], "command": "insert_gist_list" },
	  { "keys": ["ctrl+x", "ctrl+]"], "command": "gist_add_file" },


## Plugins


## Settings
### User Settings

	{
		"color_scheme": "Packages/Tomorrow Color Schemes/Tomorrow-Night-Eighties.tmTheme",
		"fade_fold_buttons": false,
		"fold_buttons": true,
		"font_face": "YaHei Consolas Hybrid",
		"font_options":
		[
			"subpixel_antialias"
		],
		"font_size": 13.0,
		"gutter": true,
		"highlight_modified_tabs": true,
		"ignored_packages":
		[
			"Toggle Read-Only",
			"SublimeCodeIntel",
			"Chrome Apps and Extensions",
			"ZenCoding",
			"Switch",
			"ColorSchemeSelector",
			"SublimeLinter"
		],
		"line_numbers": true,
		"margin": 4,
		"word_wrap": true,
		"open_files_in_new_window": false,
		"theme": "Soda Light.sublime-theme"
	}

### user keybinds 备忘

	//perfect! emacs-like-keybindings~~>_<
	[

	  //vintage

	  { "keys": ["escape","escape"], "command": "exit_insert_mode",
	    "context":
	    [
	      { "key": "setting.command_mode", "operand": false },
	      { "key": "setting.is_widget", "operand": false }
	    ]
	  },

	  { "keys": ["escape","escape"], "command": "exit_visual_mode",
	    "context":
	    [
	      { "key": "setting.command_mode"},
	      { "key": "num_selections", "operand": 1},
	      { "key": "selection_empty", "operator": "equal", "operand": false, "match_all": false }
	    ]
	  },

	  { "keys": ["escape","escape"], "command": "hide_auto_complete", "context":
	    [
	      { "key": "auto_complete_visible", "operator": "equal", "operand": true }
	    ]
	  },

	  { "keys": ["escape","escape"], "command": "vi_cancel_current_action", "context":
	    [
	      { "key": "setting.command_mode" },
	      { "key": "selection_empty", "operator": "equal", "operand": true, "match_all": false },
	      { "key": "vi_has_input_state" }
	    ]
	  },


	{ "keys": ["escape"], "command": "single_selection", "context":
	    [
	      { "key": "num_selections", "operator": "not_equal", "operand": 1 }
	    ]
	  },
	  { "keys": ["escape"], "command": "clear_fields", "context":
	    [
	      { "key": "has_next_field", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["escape"], "command": "clear_fields", "context":
	    [
	      { "key": "has_prev_field", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["escape"], "command": "hide_panel", "args": {"cancel": true},
	    "context":
	    [
	      { "key": "panel_visible", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["escape"], "command": "hide_overlay", "context":
	    [
	      { "key": "overlay_visible", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["escape"], "command": "hide_auto_complete", "context":
	    [
	      { "key": "auto_complete_visible", "operator": "equal", "operand": true }
	    ]
	  },
	  
	  { "keys": ["h"], "command": "enter_insert_mode",
	    "context":
	    [
	      {"key": "setting.command_mode"},
	      {"key": "selection_empty"}
	    ]
	  },
	  { "keys": ["i"], "command": "set_motion", "args": {
	    "motion": "move",
	    "motion_args": {"by": "lines", "forward": false, "extend": true },
	    "linewise": true },
	    "context": [{"key": "setting.command_mode"}]
	  },
	  { "keys": ["k"], "command": "set_motion", "args": {
	    "motion": "move",
	    "motion_args": {"by": "lines", "forward": true, "extend": true },
	    "linewise": true },
	    "context": [{"key": "setting.command_mode"}]
	  },
	  { "keys": ["j"], "command": "set_motion", "args": {
	    "motion": "vi_move_by_characters_in_line",
	    "motion_args": {"forward": false, "extend": true }},
	    "context": [{"key": "setting.command_mode"}]
	  },


	  { "keys": ["H"], "command": "enter_insert_mode", "args":
	    {"insert_command": "vi_move_to_first_non_white_space_character"},
	    "context": [{"key": "setting.command_mode"}]
	  },

	  { "keys": ["H"], "command": "enter_insert_mode",
	    "args": {"insert_command": "shrink_selections_to_beginning"},
	    "context": [
	      {"key": "setting.command_mode"},
	      {"key": "selection_empty", "operator": "equal", "operand": false}
	    ]
	  },
	  //   { "keys": ["I"], "command": "enter_insert_mode", "args":
	  //   {"insert_command": "vi_move_to_first_non_white_space_character"},
	  //   "context": [{"key": "setting.command_mode"}]
	  // },

	  // { "keys": ["I"], "command": "enter_insert_mode",
	  //   "args": {"insert_command": "shrink_selections_to_beginning"},
	  //   "context": [
	  //     {"key": "setting.command_mode"},
	  //     {"key": "selection_empty", "operator": "equal", "operand": false}
	  //   ]
	  // },
	  { "keys": ["I"], "command": "set_motion", "args": {
	    "motion": "move_caret_to_screen_top",
	    "motion_args": {"repeat": 1},
	    "linewise": true },
	    "context": [{"key": "setting.command_mode"}]
	  },
	  { "keys": ["K"], "command": "join_lines", "context": [{"key": "setting.command_mode"}] },
	  { "keys": ["J"], "command": "set_motion", "args": {
	    "motion": "move_caret_to_screen_top",
	    "motion_args": {"repeat": 1},
	    "linewise": true },
	    "context": [{"key": "setting.command_mode"}]
	  },

	  //gist
	  { "keys": ["ctrl+x", "ctrl+i"], "command": "gist" },
	  { "keys": ["ctrl+x", "ctrl+p"], "command": "gist_private" },
	  { "keys": ["ctrl+x", "ctrl+s"], "command": "gist_update_file" },
	  { "keys": ["ctrl+x", "ctrl+o"], "command": "gist_list" },
	  { "keys": ["ctrl+x", "ctrl+["], "command": "insert_gist_list" },
	  { "keys": ["ctrl+x", "ctrl+]"], "command": "gist_add_file" },





	  /////>>>>>>>>>>>>>>>>>>>>>>>>>>>>    sublime setting    >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
	  //替换原有的ctrl+k为ctrl+x
	  { "keys": ["ctrl+x", "ctrl+z"], "command": "toggle_side_bar" },
	  { "keys": ["ctrl+x", "ctrl+u"], "command": "upper_case" },
	  { "keys": ["ctrl+x", "ctrl+alt+u"], "command": "lower_case" },
	  { "keys": ["ctrl+x", "ctrl+space"], "command": "set_mark" },
	  // { "keys": ["ctrl+x", "ctrl+a"], "command": "select_to_mark" },
	  { "keys": ["ctrl+x", "ctrl+w"], "command": "delete_to_mark" },
	  // { "keys": ["ctrl+x", "ctrl+x"], "command": "swap_with_mark" },
	  { "keys": ["ctrl+x", "ctrl+y"], "command": "yank" },
	  { "keys": ["ctrl+x", "ctrl+backspace"], "command": "run_macro_file", "args": {"file": "Packages/Default/Delete to Hard BOL.sublime-macro"} },
	  { "keys": ["ctrl+x", "ctrl+g"], "command": "clear_bookmarks", "args": {"name": "mark"} },
	  { "keys": ["ctrl+x", "ctrl+c"], "command": "show_at_center" },
	  { "keys": ["ctrl+x", "ctrl+1"], "command": "fold_by_level", "args": {"level": 1} },
	  { "keys": ["ctrl+x", "ctrl+2"], "command": "fold_by_level", "args": {"level": 2} },
	  { "keys": ["ctrl+x", "ctrl+3"], "command": "fold_by_level", "args": {"level": 3} },
	  { "keys": ["ctrl+x", "ctrl+4"], "command": "fold_by_level", "args": {"level": 4} },
	  { "keys": ["ctrl+x", "ctrl+5"], "command": "fold_by_level", "args": {"level": 5} },
	  { "keys": ["ctrl+x", "ctrl+6"], "command": "fold_by_level", "args": {"level": 6} },
	  { "keys": ["ctrl+x", "ctrl+7"], "command": "fold_by_level", "args": {"level": 7} },
	  { "keys": ["ctrl+x", "ctrl+8"], "command": "fold_by_level", "args": {"level": 8} },
	  { "keys": ["ctrl+x", "ctrl+9"], "command": "fold_by_level", "args": {"level": 9} },
	  { "keys": ["ctrl+x", "ctrl+0"], "command": "unfold_all" },
	  { "keys": ["ctrl+x", "ctrl+t"], "command": "fold_tag_attributes" },
	  
	  
	  //原有命令, 未改
	  { "keys": ["ctrl+p"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true} },
	  { "keys": ["ctrl+shift+p"], "command": "show_overlay", "args": {"overlay": "command_palette"} },
	  { "keys": ["alt+p"], "command": "show_overlay", "args": {"overlay": "command_palette"} },
	  
	  //{ "keys": ["alt+h"], "command": "move", "args": {"by": "subwords", "forward": false} },
	  //{ "keys": ["alt+l"], "command": "move", "args": {"by": "subword_ends", "forward": true} },
	  //{ "keys": ["alt+shift+h"], "command": "move", "args": {"by": "subwords", "forward": false, "extend": true} },
	  //{ "keys": ["alt+shift+l"], "command": "move", "args": {"by": "subword_ends", "forward": true, "extend": true} },

	  { "keys": ["ctrl+pagedown"], "command": "next_view" },
	  { "keys": ["ctrl+pageup"], "command": "prev_view" },
	  { "keys": ["ctrl+tab"], "command": "next_view_in_stack" },
	  { "keys": ["ctrl+shift+tab"], "command": "prev_view_in_stack" },

	  { "keys": ["ctrl+shift+l"], "command": "split_selection_into_lines" },

	  

	//>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>



	  //todo keys
	  { "command": "todo", "keys": [ "ctrl+alt+t" ] },
	  { "keys": ["ctrl+shift+t"], "command": "reopen_last_file" },

	  //和ctrl+d有关的, useful!
	  { "keys": ["ctrl+shift+d"], "command": "duplicate_line" }, //复制行
	  { "keys": ["ctrl+x", "ctrl+d"], "command": "find_under_expand_skip" }, //跳过当前
	  { "keys": ["ctrl+d"], "command": "find_under_expand" },
	  //快速选择多个词, alt+f3, f3跳转
	  
	  //这个很好, 扩展选区
	  //shift+l被占用了, 所以用ctrl+alt+l代替, 用shift+i,k调整. 注意ctrl+alt+k被占用而且l代表line, 很好
	  { "keys": ["ctrl+alt+l"], "command": "expand_selection", "args": {"to": "line"} },
	  { "keys": ["ctrl+shift+space"], "command": "expand_selection", "args": {"to": "scope"} },
	  { "keys": ["ctrl+shift+9"], "command": "expand_selection", "args": {"to": "brackets"} },
	  { "keys": ["ctrl+shift+n"], "command": "expand_selection", "args": {"to": "indentation"} },
	  // { "keys": ["ctrl+shift+a"], "command": "expand_selection", "args": {"to": "tag"} },
	  //括号匹配
	  { "keys": ["ctrl+9"], "command": "move_to", "args": {"to": "brackets"} },   
	  // { "keys": ["ctrl+shift+h"], "command": "replace_next" },
	  
	  { "keys": ["ctrl+alt+u"], "command": "convert_to_utf8", "args": {"encoding": "UTF-8", "stamp": "0" } },


	  // { "keys": ["ctrl+alt+a"], "command": "alignment" },


	//>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>    sublemacs    >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
	//>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

	  { "keys": ["alt+q"], "command": "wrap_lines" },
	  { "keys": ["alt+q"], "command": "sbp_wrap_paragraph"},
	  // { "keys": ["ctrl+o"], "command": "sbp_open_line" },


	  // Emacs style
	  // * Automatic mode detection like it's done in Emacs using prefixes ``-*- c++ -*-``
	  // * Find file at point ``M-x f f a p`` opens the file your current cursor points to

	  //toggle comment
	  { "keys": ["alt+;"], "command": "toggle_comment" },
	  { "keys": ["ctrl+;"], "command": "toggle_comment", "args": { "block": false } },
	  { "keys": ["ctrl+shift+;"], "command": "toggle_comment", "args": { "block": true } },
	  
	  //select all
	  { "keys": ["ctrl+x", "ctrl+a"], "command": "select_all" },
	  { "keys": ["ctrl+x","h"], "command": "select_all"},
	  
	  //delete
	  { "keys": ["ctrl+h"], "command": "left_delete" },
	  { "keys": ["alt+h"], "command": "delete_word", "args": { "forward": false } },
	  { "keys": ["ctrl+o"], "command": "right_delete" },
	  { "keys": ["alt+o"], "command": "delete_word", "args": { "forward": true } },
	  { "keys": ["ctrl+shift+h"], "command": "run_macro_file", "args": {"file": "Packages/Default/Delete to Hard BOL.sublime-macro"}},
	  
	  { "keys": ["alt+delete"], "command": "delete_word", "args": { "forward": true } },
	  { "keys": ["ctrl+backspace"], "command": "delete_word", "args": { "forward": false } },
	  { "keys": ["alt+backspace"], "command": "delete_word", "args": { "forward": false } },
	  { "keys": ["super+backspace"], "command": "delete_word", "args": { "forward": false } },
	  
	  //undo and redo
	  { "keys": ["ctrl+/"], "command": "undo"},
	  { "keys": ["ctrl+shift+/"], "command": "redo"},
	  { "keys": ["ctrl+u"], "command": "undo"},
	  { "keys": ["ctrl+shift+u"], "command": "redo"},
	  // { "keys": ["ctrl+shift+/"], "command": "soft_redo" },
	  { "keys": ["alt+z"], "command": "redo"},
	  { "keys": ["ctrl+_"], "command": "undo"}, // consistency with the Mac

	  //move
	  { "keys": ["ctrl+n"], "command": "move", "args": {"by": "lines", "forward": true} },
	  // { "keys": ["ctrl+p"], "command": "move", "args": {"by": "lines", "forward": false} },

	  { "keys": ["ctrl+j"], "command": "move", "args": {"by": "characters", "forward": false} },
	  { "keys": ["ctrl+l"], "command": "move", "args": {"by": "characters", "forward": true} },
	  { "keys": ["ctrl+i"], "command": "move", "args": {"by": "lines", "forward": false} },
	  { "keys": ["ctrl+k"], "command": "move", "args": {"by": "lines", "forward": true} },
	  
	  { "keys": ["alt+j"], "command": "move", "args": {"by": "words", "forward": false} },
	  { "keys": ["alt+l"], "command": "move", "args": {"by": "word_ends", "forward": true} },
	  { "keys": ["alt+i"], "command": "move", "args": {"by": "pages", "forward": false} },
	  { "keys": ["alt+k"], "command": "move", "args": {"by": "pages", "forward": true} },


	  { "keys": ["ctrl+shift+j"], "command": "move", "args": {"by": "characters", "forward": false, "extend": true} },
	  { "keys": ["ctrl+shift+l"], "command": "move", "args": {"by": "characters", "forward": true, "extend": true} },
	  { "keys": ["ctrl+shift+i"], "command": "move", "args": {"by": "lines", "forward": false, "extend": true} },
	  { "keys": ["ctrl+shift+k"], "command": "move", "args": {"by": "lines", "forward": true, "extend": true} },

	  { "keys": ["alt+shift+j"], "command": "move", "args": {"by": "words", "forward": false, "extend": true} },
	  { "keys": ["alt+shift+l"], "command": "move", "args": {"by": "word_ends", "forward": true, "extend": true} },

	  { "keys": ["ctrl+alt+i"], "command": "select_lines", "args": {"forward": false} },
	  { "keys": ["ctrl+alt+k"], "command": "select_lines", "args": {"forward": true} },




	  { "keys": ["ctrl+a"], "command": "move_to", "args": {"to": "bol", "extend": false} },
	  { "keys": ["ctrl+e"], "command": "move_to", "args": {"to": "eol", "extend": false} },
	  { "keys": ["ctrl+e"], "command": "move_to", "args": {"to": "eol", "extend": true}, "context":
	    [
	      { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },
	  
	  { "keys": ["shift+ctrl+a"], "command": "move_to", "args": {"to": "bol", "extend": true} },
	  { "keys": ["shift+ctrl+e"], "command": "move_to", "args": {"to": "eol", "extend": true} },

	  { "keys": ["pageup"], "command": "move", "args": {"by": "pages", "forward": false} },
	  { "keys": ["pagedown"], "command": "move", "args": {"by": "pages", "forward": true} },
	  { "keys": ["alt+,"], "command": "move", "args": {"by": "pages", "forward": false} },
	  { "keys": ["alt+."], "command": "move", "args": {"by": "pages", "forward": true} },
	  { "keys": ["shift+pageup"], "command": "move", "args": {"by": "pages", "forward": false, "extend": true} },
	  { "keys": ["shift+pagedown"], "command": "move", "args": {"by": "pages", "forward": true, "extend": true} },

	  { "keys": ["ctrl+home"], "command": "move_to", "args": {"to": "bof", "extend": false} },
	  { "keys": ["ctrl+end"], "command": "move_to", "args": {"to": "eof", "extend": false} },
	  { "keys": ["ctrl+shift+home"], "command": "move_to", "args": {"to": "bof", "extend": true} },
	  { "keys": ["ctrl+shift+end"], "command": "move_to", "args": {"to": "eof", "extend": true} },

	  { "keys": ["ctrl+alt+,"], "command": "move_to", "args": {"to": "bof", "extend": false}},
	  { "keys": ["ctrl+alt+."], "command": "move_to", "args": {"to": "eof", "extend": false}},
	  { "keys": ["shift+alt+,"], "command": "move_to", "args": {"to": "bof", "extend": false}},
	  { "keys": ["shift+alt+."], "command": "move_to", "args": {"to": "eof", "extend": false}},
	  

	  { "keys": ["ctrl+up"], "command": "scroll_lines", "args": {"amount": 1.0 } },
	  { "keys": ["ctrl+down"], "command": "scroll_lines", "args": {"amount": -1.0 } },

	  // { "keys": ["ctrl+l"], "command": "sbp_recenter_in_view" },
	 
	  // Kill Ring handling
	  //cut  (only cut, can't kill line)
	  { "keys": ["ctrl+w"], "command": "sbp_delete_to_mark" },
	  { "keys": ["ctrl+x","ctrl+x"], "command": "sbp_delete_to_mark" },
	  //copy or copy line
	  { "keys": ["ctrl+c"], "command": "sbp_kill_ring_save" },
	  { "keys": ["alt+w"], "command": "sbp_kill_ring_save" },
	  //kill line  (just like emacs, no & no need one key kill line)
	  { "keys": ["ctrl+m"], "command": "sbp_kill_line"},
	  { "keys": ["alt+m"], "command": "sbp_kill_to_end_of_sentence"},
	  //paste& yank choice
	  { "keys": ["ctrl+y"], "command": "paste" },
	  { "keys": ["alt+y"], "command": "sbp_yank_choice" },
	  { "keys": ["ctrl+v"], "command": "paste" },
	  { "keys": ["alt+v"], "command": "sbp_yank_choice" },

	  
	  //set mark
	  { "keys": ["ctrl+space"], "command": "sbp_set_mark" },
	  { "keys": ["ctrl+g"], "command": "sbp_cancel_mark" },


	  //move with mark
	  { "keys": ["ctrl+l"], "command": "move", "args": {"by": "characters", "forward": true, "extend": true}, "context": 
	    [
	        { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+j"], "command": "move", "args": {"by": "characters", "forward": false, "extend": true}, "context":
	    [
	      { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["alt+j"], "command": "move", "args": {"by": "words", "forward": false, "extend": true}, "context": 
	    [
	        { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ] 
	  },

	  { "keys": ["alt+l"], "command": "move", "args": {"by": "word_ends", "forward": true, "extend": true}, "context": 
	    [
	        { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },

	  { "keys": ["ctrl+k"], "command": "move", "args": {"by": "lines", "forward": true, "extend": true}, "context": 
	    [
	        { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+i"], "command": "move", "args": {"by": "lines", "forward": false, "extend": true}, "context":
	    [
	        { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+space"], "command": "sbp_cancel_mark", "context" :
	    [
	        { "key": "sbp_emacs_has_mark", "operator": "equal", "operand": true }
	    ]
	  },

	  // Search and Replace
	  { "keys": ["ctrl+r"], "command": "show_panel", "args": {"panel": "incremental_find", "reverse":true} },
	  { "keys": ["ctrl+s"], "command": "show_panel", "args": {"panel": "incremental_find", "reverse":false} },
	  { "keys": ["ctrl+alt+r"], "command": "show_panel", "args": {"panel": "replace"} },
	  { "keys": ["super+r"], "command": "show_panel", "args": {"panel": "replace"} },

	  // Goto stuff
	  { "keys": ["ctrl+f"], "command": "show_panel", "args": {"panel": "find"} },
	  { "keys": ["ctrl+x", "ctrl+f"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true} },
	  // { "keys": ["alt+f"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true} },
	  { "keys": ["alt+g"], "command": "show_overlay", "args": {"overlay": "goto", "show_files": true, "text" : ":"}},
	  { "keys": ["ctrl+alt+g"], "command": "show_overlay", "args": {"overlay":"goto", "show_files" : false, "text": "@"}},
	  { "keys": ["ctrl+x", "b"], "command": "next_view" },
	  { "keys": ["ctrl+x", "ctrl+b"], "command": "goto_open_file"},


	  { "keys": ["ctrl+x", "o"], "command": "sbp_cycle_focus_group"},

	  {
	    "keys": ["ctrl+x", "2"],
	    "command": "set_layout",
	    "args":
	    {
	      "cols": [0.0, 1.0],
	      "rows": [0.0, 0.5, 1.0],
	      "cells": [[0, 0, 1, 1], [0, 1, 1, 2]]
	    }
	  },
	  {
	    "keys": ["ctrl+x", "1"],
	    "command": "set_layout",
	    "args":
	    {
	      "cols": [0.0, 1.0],
	      "rows": [0.0, 1.0],
	      "cells": [[0, 0, 1, 1]]
	    }
	  },
	  {
	    "keys": ["ctrl+x", "3"],
	    "command": "set_layout",
	    "args":
	    {
	      "cols": [0.0, 0.5, 1.0],
	      "rows": [0.0, 1.0],
	      "cells": [[0, 0, 1, 1], [1, 0, 2, 1]]
	    }
	  },

	  // { "keys": ["ctrl+1"], "command": "focus_group", "args": { "group": 0 } },

	  // Completion
	  { "keys": ["alt+/"], "command": "auto_complete" },
	  { "keys": ["alt+/"], "command": "replace_completion_with_auto_complete", "context":
	    [
	      { "key": "last_command", "operator": "equal", "operand": "insert_best_completion" },
	      { "key": "auto_complete_visible", "operator": "equal", "operand": false },
	      { "key": "setting.tab_completion", "operator": "equal", "operand": true }
	    ]
	  },

	  // Aborter
	  //origin
	  { "keys": ["ctrl+g"], "command": "single_selection", "context":
	    [
	      { "key": "num_selections", "operator": "not_equal", "operand": 1 }
	    ]
	  },
	  { "keys": ["ctrl+g"], "command": "clear_fields", "context":
	    [
	      { "key": "has_next_field", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+g"], "command": "clear_fields", "context":
	    [
	      { "key": "has_prev_field", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+g"], "command": "hide_panel", "args": {"cancel": true},
	    "context":
	    [
	      { "key": "panel_visible", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+g"], "command": "hide_overlay", "context":
	    [
	      { "key": "overlay_visible", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+g"], "command": "hide_auto_complete", "context":
	    [
	      { "key": "auto_complete_visible", "operator": "equal", "operand": true }
	    ]
	  },


	  //sublemacs
	  { "keys": ["ctrl+g"], "command": "hide_overlay", "context":
	    [
	      { "key": "overlay_visible", "operator": "equal", "operand": true }
	    ]
	  },
	   { "keys": ["ctrl+g"], "command": "hide_auto_complete", "context":
	    [
	      { "key": "auto_complete_visible", "operator": "equal", "operand": true }
	    ]
	  },
	  { "keys": ["ctrl+g"], "command": "hide_panel", "context":
	    [
	      { "key": "panel_visible", "operator": "equal", "operand": true }
	    ]
	  },

	  // Rectangles
	  { "keys": ["ctrl+x", "r", "t"], "command": "sbp_rectangle_insert" },
	  { "keys": ["ctrl+x", "r", "d"], "command": "sbp_rectangle_delete" },

	  // Registers
	  { "keys": ["ctrl+x", "r", "s"], "command": "sbp_register_store" },
	  { "keys": ["ctrl+x", "r", "i"], "command": "sbp_register_insert" },

	  // Do it my way
	  { "keys": ["ctrl+x", "k"], "command": "close" },
	  { "keys": ["ctrl+x", "ctrl+c"], "command": "exit"},
	  { "keys": ["ctrl+x", "ctrl+s"], "command": "save"},

	  // Other Emacs features
	  { "keys": ["ctrl+x", "ctrl+j"], "command": "sbp_find_file_at_point" },

	  //origin tab reindent
	  // { "keys": ["tab"], "command": "reindent", "context":
	  //   [
	  //     { "key": "setting.auto_indent", "operator": "equal", "operand": true },
	  //     { "key": "selection_empty", "operator": "equal", "operand": true, "match_all": true },
	  //     { "key": "preceding_text", "operator": "regex_match", "operand": "^$", "match_all": true },
	  //     { "key": "following_text", "operator": "regex_match", "operand": "^$", "match_all": true }
	  //   ]
	  // },
	    // Emacs style tabs  (use shift tab) 
	  { "keys": ["tab"], "command": "reindent",  "context": [
	    { "key": "panel_has_focus",  "operand": false },
	    { "key": "auto_complete_visible", "operand": false },
	    { "key": "has_next_field", "operand": false },
	    { "key": "overlay_visible", "operand": false }

	    ]
	  },

	  { "keys": ["tab"], "command": "reindent",  "context": [
	    
	    { "key": "selector", "operator": "nonequal", "operand": "text.html.markdown" }

	    ]
	  },
	  
	//>>>>>>>>>>>>>>>>>>>>>>>>>>>    sublemacsend    >>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>

	//table editor

	 { "keys": ["ctrl+alt+j"], "command": "table_editor_join_lines", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "(\\|)|(\\+)", "match_all": true }
	        ]
	    },

	{ "keys": ["ctrl+x","-"], "command": "table_editor_insert_single_hline", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "$", "match_all": true }
	        ]
	    },
	    { "keys": ["ctrl+x","="], "command": "table_editor_insert_double_hline", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "$", "match_all": true }
	        ]
	    },
	    { "keys": ["ctrl+x","enter"], "command": "table_editor_hline_and_move", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true },
	            { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*((\\|)|(\\+))", "match_all": true },
	            { "key": "following_text", "operator": "regex_contains", "operand": "$", "match_all": true }
	        ]
	    },
	    { "keys": ["ctrl+x","|"], "command": "table_editor_csv_to_table", "context":
	        [
	            { "key": "setting.enable_table_editor", "operator": "equal", "operand": true, "match_all": true }
	        ]
	    },


	//smart markdown
	{ "keys": ["tab"], "command": "smart_folding", "context":
	    [
	      { "key": "selector", "operator": "equal", "operand": "markup.heading.markdown" }
	    ]
	  },
	  { "keys": ["shift+tab"], "command": "global_folding", "context":
	      [
	      { "key": "selector", "operator": "equal", "operand": "text.html.markdown" }
	    ]
	  },
	  { "keys": ["enter"], "command": "smart_list", "context":
	    [
	      { "key": "selector", "operator": "equal", "operand": "text.html.markdown" },
	      { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*([-+*]|\\d+\\.+)\\s+" }
	    ]
	  },
	  { "keys": ["enter"], "command": "smart_list", "context":
	    [
	        { "key": "selector", "operator": "equal", "operand": "text.html.markdown" },
	      { "key": "selector", "operator": "equal", "operand": "markup.list" }
	    ]
	  },
	  { "keys": ["tab"], "command": "smart_table",
	    "args": {"forward": true}, "context":
	    [
	      { "key": "selector", "operator": "equal", "operand": "text.html.markdown" },
	      { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*(\\||\\+[-=])",
	        "match_all": true}
	    ]
	  },
	  { "keys": ["tab"], "command": "smart_table",
	    "args": {"forward": true}, "context":
	    [
	      { "key": "selector", "operator": "equal", "operand": "text.html.markdown" },
	      { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*" },
	      { "key": "following_text", "operator": "regex_contains", "operand": "\\s*(\\||\\+[-=])",
	        "match_all": true}
	    ]
	  },
	  { "keys": ["shift+tab"], "command": "smart_table",
	    "args": {"forward": false}, "context":
	    [
	      { "key": "selector", "operator": "equal", "operand": "text.html.markdown" },
	      { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*(\\||\\+[-=])",
	        "match_all": true}
	    ]
	  },
	  { "keys": ["shift+tab"], "command": "smart_table",
	    "args": {"forward": false}, "context":
	    [
	      { "key": "selector", "operator": "equal", "operand": "text.html.markdown" },
	      { "key": "preceding_text", "operator": "regex_contains", "operand": "^\\s*" },
	      { "key": "following_text", "operator": "regex_contains", "operand": "\\s*(\\||\\+[-=])",
	        "match_all": true}
	    ]
	  },

	//>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>>
	//ctags

	{
	    "command": "navigate_to_definition",
	    "keys": ["ctrl+t", "ctrl+t"]
	  },
	  {
	    "command": "navigate_to_definition",
	    "keys": ["ctrl+period"]
	  },
	  {
	    "command": "search_for_definition",
	    "keys": ["ctrl+t", "ctrl+y"]
	  },
	  {
	    "command": "jump_back",
	    "keys": ["ctrl+t", "ctrl+b"]
	  },
	  {
	    "command": "jump_back",
	    "keys": ["ctrl+comma"]
	  },
	  {
	    "command": "jump_back",
	    "args": {"to": "last_modification"},
	    "keys": ["ctrl+t", "ctrl+m"]
	  },
	  {
	    "command": "rbeuild_tags",
	    "keys": ["ctrl+t", "ctrl+r"]
	  }
	,  {
	    "command": "show_symbols",
	    "context": [
	      {
	        "key": "selector",
	        "match_all": true,
	        "operand": "source -source.css",
	        "operator": "equal"
	      }
	    ],
	    "keys": ["alt+s"]
	  },
	  {
	    "command": "show_symbols",
	    "args": {"type": "multi"},
	    "context": [
	      {
	        "key": "selector",
	        "match_all": true,
	        "operand": "source -source.css",
	        "operator": "equal"
	      }
	    ],
	    "keys": ["alt+shift+s"]
	  },
	  {
	    "command": "show_symbols",
	    "args": {"type": "lang"},
	    "context": [
	      {
	        "key": "selector",
	        "match_all": true,
	        "operand": "source -source.css",
	        "operator": "equal"
	      }
	    ],
	    "keys": ["ctrl+alt+shift+s"]
	  },
	  { // override current default
	    "command": "transpose",
	    "context": [
	      { "key": "num_selections", "operator": "not_equal", "operand": 1 }
	    ],
	    "keys": ["ctrl+t"]
	  }


	  
	]
