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


问题一：
error: src refspec remote does not match any.
解决处理办法
git push origin HEAD:master




