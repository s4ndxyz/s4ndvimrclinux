本版本是我使用Vim一周年的纪念版，也是最后一版，以后不再更新，还望各位朋友见谅

我是去年（2011年）5月1日正式开始使用Vim编辑器的，从此剑不离手，给予了我极大的帮助

这是我使用Vim一周年的感悟：http://www.ruchee.com/code/tools/vim/vim_one_year.html

望有缘人能通过我发布的这些集成版本快速入门，步入Vim殿堂，提高编码效率，享受编码乐趣

经过着色的配置文件请访问下面的链接

http://www.ruchee.com/code/tools/vim/vimrc.shtml

完整配置的下载地址见本文末尾

-----------------------------------------

相比4月1日那一版，本版本并没有太大的变化，只是上一版侧重于Ruby/Rails的开发，而这一版偏重于Python/Django

所以鉴于此，上一版的Vim2012-04-01.7z和当前版本的Vim2012-05-01.7z文件会永久保存在我的下载目录，以供有需者随时下载

考虑到VimWiki使用的人并不多，所以本版本对其进行了移除，此外还有其他部分插件也进行了删减

上一版的保存快捷键是Ctrl + S，这一版换成了jj，还望注意

此外，如果源文件路径含有中文字符，那么调用Taglist是显示不出函数列表的，所以请新人注意，路径不要使用中文（这也是基本的常识）

老规矩，所有常用的按键说明全部写在了配置文件的最前面，Windows下为_vimrc，Linux下为.vimrc

-----------------------------------------

本版本的主要功能：

01、支持常规的语法高亮、代码缩进、每行80个字符提示
02、支持括号、引号自动匹配
03、支持单源文件一键编译、运行 [已配置支持C/C++、Java、Haskell、Lua、Perl、Python、Ruby]
04、支持一键载入语法模板
05、集成snipMate，支持tab键补全 [已完整配置支持的语种有C/C++、Python/Django、Ruby/Rails]
06、集成zencoding，支持网页的快速编码
07、集成minibufexpl、NERD_tree、taglist等常规插件，便于开发工程级项目
08、支持GTK+和Qt的语法高亮
09、集成txtbrowser，对普通的txt文本文件也有良好的渲染
10、对于HTML文件，默认载入Django Template语法高亮模式，便于Python/Django开发
11、集成Powerline，支持状态栏彩色显示
12、支持ctags函数跳转 [Linux && Cygwin用户需要安装有ctags才能使用]

-----------------------------------------

更多功能请自行查看Vim配置文件 [Windows为_vimrc，Linux和Cygwin为.vimrc]

zencoding简易的使用说明请参考：
http://www.ruchee.com/code/tools/vim/zencoding.html

snipMate支持的关键字，请自行查看vimfiles/snippets目录下的各个文件（Linux对应的目录为.vim/snippets），你也可以自行修改和配置

下面是配置的具体安装方法，分Windows和Linux && Cygwin两个版本，请根据需要参考

-----------------------------------------

Windows下的安装方法

01、访问http://www.vim.org/download.php#pc下载最新的Gvim

02、安装Gvim到任意目录，这儿为方便讲解，我假定你安装到了D:\Apps\Gvim

03、将D:\Apps\Gvim\vim73目录加入环境变量 [不知何为环境变量者，请Google]

04、删除Gvim安装目录下的vimfiles目录

05、复制提供的vimfiles目录到D:\Apps\Gvim下，取代已删目录的位置

06、将提供的小工具软件全部复制到D:\Apps\Gvim\vim73目录下

07、复制_vimrc到D:\Apps\Gvim进行替换

08、复制Monaco.ttf到C:\WINDOWS\Fonts目录下进行字体的安装

09、使用任意文本编辑器打开_vimrc，将名字、邮箱、网址等全部替换为你自己的信息，如遇路径不同也全部替换为你本机的实际路径

10、然后。。。然后就大功告成了，接下只需学习如何使用而已，使用说明全部集中在_vimrc文件的头部

-----------------------------------------

Linux && Cywgin下的安装方法

01、请确认已安装Vim，这儿不提供Vim的安装指导，如有需要请Google

02、删除家目录的.vim文件夹和.vimrc文件，如果没有则不需要执行删除动作 [使用命令 rm -rf .vim .vimrc]

03、复制Linux_Cygwin目录下的所有文件到家目录 [在下载的Linux_Cygwin文件夹上打开终端，然后执行命令 cp -r . ~]

04、使用任意文本编辑器打开.vimrc，将名字、邮箱、网址等全部替换为你自己的信息，如遇路径不同也全部替换为你本机的实际路径

05、如此这般就配置好了，尽情享受编码的乐趣吧，使用说明全部集中在.vimrc文件的头部

-----------------------------------------

ctags简易的使用说明，这儿以C/C++为例

01、首先确保系统能够找到ctags.exe，也就是ctags.exe添加到了系统环境变量

02、以MinGW为例，到编译器安装目录的include目录（比如C:\MinGW\include）执行命令 ctags -R --languages=c,c++

03、在_vimrc文件中添加一行 set tags+=C:\MinGW\include\tags

04、以后编辑C/C++源文件时，键入一小部分字符，然后按Ctrl + P即可拥有C/C++的代码提示

05、将光标移到某个函数名上，按Ctrl + ]，Vim将自动跳转到该函数的定义，按Ctrl + T返回

以上只是ctags简单的用法，更专业的介绍请Google

-----------------------------------------

资料目录提供了几份实用的Vim教程和图解，希望能给你学习Vim的使用带来帮助

附件下载地址：http://www.ruchee.com/download/Vim2012-05-01.7z

上一版本的下载地址：http://www.ruchee.com/download/Vim2012-04-01.7z

-----------------------------------------

附小广告一枚，欢迎相应技术领域的爱好者加入以下Q群

[Python高级编程群已有490多人，RoR高级编程群已有530多人，欢迎各位]

[提交加群申请时注明自己是某某程序员即可，如 Pythoner、Rubyer、Haskeller]


1、Ruby on Rails高级编程：154112964

2、Haskell函数式高级编程：72874436

3、Python高级编程：195132894

4、Python Web编程：182399563

-----------------------------------------

  Author: Ruchee
   Email: my@ruchee.com
 WebSite: http://www.ruchee.com
    Date: 2012-05-01
