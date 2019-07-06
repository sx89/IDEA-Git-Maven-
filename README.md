# IDEA-Git-Maven-
磨刀不误砍柴工,整理一些拓展知识,基础的网上一大片,就不整理了

## IDEA
+ 忽略大小写补全代码:

![](pic/Snipaste_2019-07-06_21-20-02.jpg)

+ 历史粘贴板

![](pic/Snipaste_2019-07-06_09-00-00_看图王.jpg)

+ ctrl + alt + 上下键  

光标上次出现的位置

+ ctrl + alt + 左右键

代码的来回跳转

+  ctrl + shift / alt + shift   + 上下键  

代码行的上下移动

+ ctrl + alt + t 

选中代码块被 ?  包裹

![](pic/Snipaste_2019-07-06_09-05-37_看图王.jpg)

+ ctrl + j 

常见代码块快速生成

还有一些常见的缩写  
psf(priavte  static final)  
ifn (if (not null))  
sout (system.out.println)

![](pic/Snipaste_2019-07-06_09-16-21_看图王.jpg)

+ ctrl + alt + h

查看代码引用了哪些类,和被哪些类引用 
![](pic/Snipaste_2019-07-06_09-52-21_看图王.jpg)

+ ctrl + alt + m

抽取方法出来(用于重构代码,还有一个重构神器:shift + f6 重命名代码)
+ ctrl + alt + v

自动创建变量,接受返回值

+ 条件断点

在断点上右键

+ 异常断点

![](pic/Snipaste_2019-07-06_14-52-58_看图王.png)

## Git

+ 远程覆盖本地代码

git fetch
git reset --hard origin master

+ git 撤销commit 但未push的代码

git log
git reset --hard(如果想保留修改内容而不是强制覆盖,则不加--hard) commitID

+ 撤销 为commit的修改

git status  

返回的英文里面告诉你了用什么命令撤回

+ rebase

git rebase -i HEAD~4 或者 git rebase -i  commitID(如果我想把1,2,3合并,我的commitId要写3的下一个,即4)
