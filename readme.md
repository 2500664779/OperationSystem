Git基本常用命令如下：

   mkdir：         XX (创建一个空目录 XX指目录名)

   pwd：          显示当前目录的路径。

   cd..		  返回上一级目录

   cd git	  进入某一目录

   git init          把当前的目录变成可以管理的git仓库，生成隐藏.git文件。

   git add XX       把xx文件添加到暂存区去。

   git commit –m “XX”  提交文件 –m 后面的是注释。
   
   git status        查看仓库状态

   git diff  XX      查看XX文件修改了那些内容

   git log          查看历史记录

   git reset  –hard HEAD^ 或者 git reset  –hard HEAD~ 回退到上一个版本

      (如果想回退到100个版本，使用git reset –hard HEAD~100 )

   cat XX         查看XX文件内容

   git reflog       查看历史记录的版本号id

   git checkout — XX  把XX文件在工作区的修改全部撤销。

   git rm XX          删除XX文件

   git remote add origin https://github.com/tugenhua0707/testgit 关联一个远程库

   git push –u(第一次要用-u 以后不需要) origin master 把当前master分支推送到远程库

   git clone https://github.com/tugenhua0707/testgit  从远程库中克隆

   git checkout –b dev  创建dev分支 并切换到dev分支上

   git branch  查看当前所有的分支

   git checkout master 切换回master分支

   git merge dev    在当前的分支上合并dev分支

   git branch –d dev 删除dev分支

   git branch name  创建分支

   git stash 把当前的工作隐藏起来 等以后恢复现场后继续工作

   git stash list 查看所有被隐藏的文件列表

   git stash apply 恢复被隐藏的文件，但是内容不删除

   git stash drop 删除文件

   git stash pop 恢复文件的同时 也删除文件

   git remote 查看远程库的信息

   git remote –v 查看远程库的详细信息

   git push origin master  Git会把master分支推送到远程库对应的远程分支
---------- 
gitignore 的匹配规则：
```
#以此开头的行为注释行
.a #过滤所有 .a 结尾的文件
/a/ #过滤根目录下的 a 文件夹下的所有文件
/a/do.c #过滤指定文件 /a/do.c
!lib.a #从过滤的文件中排除 lib.a
!/a/b #从过滤的文件中排除 根目录下a目录下的b文件
!.c #从过滤的文件中排除所有.c文件
/TODO #仅仅过滤项目根目录下的 TODO 文件,不包括subdir/TODO
build/ #过滤 build/目录下的所有文件
doc/*.txt #过滤doc下所有txt文件,但不包括子目录下的txt文件,如doc/server/arch.txt
```