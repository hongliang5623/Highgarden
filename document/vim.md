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
