# vim的各种技巧
##数行操作
###  删除列
> * 光标定位到要操作的地方。
> * CTRL+v 进入“可视 块”模式，选取这一列操作多少行。
> * d 删除。
 
###  插入列
插入操作和删除稍有区别
> * 光标定位到要操作的地方。
> * CTRL+v 进入“可视 块”模式，选取这一列操作多少行。
> * SHIFT+i(I) 输入要插入的内容。
> * ESC 按两次，会在每行的选定的区域出现插入的内容。

### vimrc配置
```python
  1 set nu
  2 set tabstop
  3 set nobackup
  4 set cursorline
  5 set ruler
  6 set autoindent
  7 set tabstop=8                                                                                                                                           
  8 set shiftwidth=4
  9 set softtabstop=4
 10 set expandtab
 ```
### 目前的配置
```python
"显示行号
set nu

"设置缩进tabstop
set ts=4
set shiftwidth=4
set expandtab
set ruler

"语法高亮
syntax on

"设置编码
set encoding=utf-8

"高亮搜索的关键字
set hlsearch

"设置自动缩进
"set cindent

"设置鼠标操作
set mouse=i

"设置搜索时显示结果
set incsearch

"设置插入括号时 短暂跳转到匹配的对应括号
set showmatch
set matchtime=2

"设置所在行列高亮
"set cursorline
"hi CursorLine cterm=None ctermbg=grey ctermfg=black guifg=green guibg=grey
"set cursorcolumn
"hi CursorColumn cterm=NONE ctermbg=darkred ctermfg=white guibg=darkred guifg=white

autocmd BufReadPost * if line("'\"") && line("'\"") <= line("$") | exe "normal `\"" | endif
autocmd FileType python set omnifunc=pythoncomplete#Complete
autocmd FileType html set omnifunc=htmlcomplete#CompleteTags
autocmd FileType javascript set omnifunc=javascriptcomplete#CompleteJS
autocmd FileType css set omnifunc=csscomplete#CompleteCSS
autocmd FileType xml set omnifunc=xmlcomplete#CompleteTags
```
