测试0.1



测试0.2

直接提交
no changes added to commit (use "git add" and/or "git commit -a")
1.查看状态
git status 
2.增加文件
git add ***.md
3.提交文件
git commit -m '****'   加-a参数全部提交，包含修改状态
4.push到master上
git push origin master  从本地push到master分支

5.文件的比较
git diff 

6.移除文件
然后再运行 git rm 记录此次移除文件的操作：

另外一种情况是，我们想把文件从 Git 仓库中删除（亦即从暂存区域移除），但仍然希望保留在当前工作目录中。换句话说，仅是从跟踪清单中删除。比如一些大型日志文件或者一堆.a 编译文件，不小心纳入仓库后，要移除跟踪但不删除文件，以便稍后在 .gitignore 文件中补上，用 --cached 选项即可：
git rm --cached readme.txt



7.回顾厉史日志
git log 


8.还原刚才的修改
(use "git checkout -- <file>..." to discard changes in working directory

git checkout  -- file.txt

9.查看远程 的情况
 git remote -v
 
10.添加远程仓库
git remote add pb https://github.com/lindows365/php_site.git
git remote show origin//显示远程 终端的内容

git remote rename pb paul  //改名

git remote rm paul         //删除别名


11.打标签
git tag v0.1


12.创建新分支 – git branch
git branch amazing_new_feature


13.切换分支 – git checkout

单独使用git branch，可以查看分支状态：

14.合并分支 – git merge

我们的 amazing_new_feature 分支的任务是增加一个featuer.txt。我们来创建，添加到暂存区，提交。

Shell

$ git add feature.txt
$ git commit -m "New feature complete."
1
2
$ git add feature.txt
$ git commit -m "New feature complete."
新分支任务完成了，回到master分支

Shell

$ git checkout master
1
$ git checkout master
现在去查看文件，你会发现，之前创建的feature.txt文件不见了，因为master分支上并没有feature.txt。使用git merge 把 amazing_new_feature 分支合并到master上。

Shell

$ git merge amazing_new_feature
1
$ git merge amazing_new_feature
ok! 然后再把amazing_new_feature 分支删掉吧。

Shell

$ git branch -d amazing_new_feature
1
$ git branch -d amazing_new_feature

问题一：
error: src refspec remote does not match any.
解决处理办法
git push origin HEAD:master
git push origin master --force 








