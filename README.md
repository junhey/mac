# mac开发环境

Full-Stack Developers Using MAC OS

## 通用开发

- 搜狗输入法

- QQ/WeChat

- Office

- 印象笔记

- CopyClip

- 网易云音乐

- Photoshop

- The Unachiver

- Chrome

- Alfred

- Dash

- CheatSheet

- Sublime Text/WebStorm

- iTerm

- .DS_store生成

> Mac下面压缩的时候总会自动生成 .DS_store 文件，用户可以自行选择是否需要生成，执行下面命令之后需要重启Mac生效。
```javascript
//禁止 .DS_store生成：
defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool TRUE

//恢复 .DS_store生成：
defaults delete com.apple.desktopservices DSDontWriteNetworkStores
```

- 安装HomeBrew

> HomeBrew是Mac下面的一个包管理器，方便我们安装一些Mac OS没有的UNIX工具、软件。

```
ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
- 安装HomeBrew Cask

> HomeBrew Cask依赖于Xcode以及HomeBrew，建议在装这个之前装好前面两个软件，在Terminal执行下面命令进行安装

```
brew tap caskroom/cask && brew install brew-cask
```
- 安装iTerm2

> iTerm2是一款优秀的终端软件，可用来代替系统自带的Terminal。

```
brew cask install iTerm2
```
- 安装zsh

> 什么是oh-my-zsh ？ 简单来说oh-my-zsh 是基于 zsh 的增强配置, 附带各种常用的插件。zsh 是一种Shell。

```
sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

- 安装Git
```
brew install git
```

- Github配置
```
ssh-keygen -t rsa -C "junhey@qq.com"
# Copy ssh key to github.com
subl ~/.ssh/id_rsa.pub
# Test connection
ssh -T git@github.com
# Set git config values
git config --global user.name "junhey"
git config --global user.email "junhey@qq.com"
git config --global github.user junhey
git config --global github.token your_token_here
git config --global core.editor "subl -w"
git config --global color.ui true
```

- 安装svn
```
brew install svn
```

- 更新vim
```
brew update
brew install vim
```

-SublimeText


SublimeText的最大一个组成部分就是插件，个人觉得插件能够达到精简实用最好，下面推荐一些常用的插件，仅供参考。
下面插件的安装方法
```
shift + cmd + p 打开命令面板
输入 “Package Control: Install  Package” 命令
输入 插件的名称 , 找到后回车安装
安装成功后在preferences中选择主题
Emmet （前端工程师利器，各种代码补全自动生成，更多介绍移步 官方文档）
converttoUTF8（文档转码工具）
git（git的一些操作都可以在这里进行）
sidebarenhancement（侧边栏增强，在侧边右键之后多了一些功能，挺实用的）
docblockr（文档注释，输入/*之后按一下tab就可以生成文档注释）
Bracket Highlighter（匹配括号高亮，自带的感觉高亮不强）
SCSS（sass高亮）
markdownPerview（写markdown可以command+b直接生成html预览）
evernote（配合markdownPerview就可以写markdown同步到evernote去了）
```



	