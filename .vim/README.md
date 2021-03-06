# 相关依赖

```
brew install ctags
brew install the_silver_searcher
```

> 如果系统环境已经存在`ctags`，使用上面安装的ctags可能优先级没有系统的高。
> 添加如下别名到系统环境变量中(比如将下一行添加到zsh：`~/.zshrc`配置文件中)：
> ```
> alias ctags="`brew --prefix`/bin/ctags"
> ```
> 参见这个Gist: https://gist.github.com/nazgob/1570678

# 配置Vim

1. 拷贝或者链接`.vimrc`文件到当前用户家目录下
   `ln -s /{path}/mac-config/.vimrc ~/.`
   
2. 拷贝或者链接`.gvimrc`文件到当前用户家目录下`ln -s /{path}/mac-config/.gvimrc ~/.`

3. 拷贝或者链接`.vim`目录到当前用户的家目录下
   `ln -s /{path}/mac-config/.vim ~/.`

> **注意：**  *拷贝前记得备份系统之前的数据*

3. 获取Plugins
    3.1 通过GitHub获得最新的[VundleVim/Vundle.vim](https://github.com/VundleVim/Vundle.vim)数据 
```
git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
```
    3.2 升级Plugins
打开`vim`并且运行`:PluginInstall`
