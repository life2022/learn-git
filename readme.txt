git 的学习
cat {文件名}: 查看文件
git add:  文件名暂存 
git commit -m 本次提交的说明 : 提交
git add命令实际上就是把要提交的所有修改放到暂存区（Stage），然后，执行git commit就可以一次性把暂存区的所有修改提交到分支。
(每次修改，如果不用git add到暂存区，那就不会加入到commit中)
git log: 显示从最近到最远的提交日志
git log --pretty=oneline: --pretty=oneline(嫌输出信息太多，看得眼花缭乱的，可以加上--pretty=oneline参数)

git reset --hard HEAD^ : 回退到上一个版本就是HEAD^(HEAD指向的版本就是当前版本)
git reset --hard HEAD^^ : 回退到上上一个版本就是HEAD^^
git reset --hard {commit id} : 可以指定回到未来的某个版本

git reflog: 用来记录你的每一次命令
git diff HEAD -- {文件名} : 可以查看工作区和版本库里面最新版本的区别
git status: 查看文件的提交状态

git checkout -- {文件名}: 可以丢弃工作区的修改
文件在工作区的修改全部撤销,这里有两种情况：
1、一种是文件自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
2、一种是文件已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
总之，就是让这个文件回到最近一次git commit或git add时的状态。

git reset HEAD {文件名}: 可以把暂存区的修改撤销掉（unstage），重新放回工作区
git reset命令既可以回退版本，也可以把暂存区的修改回退到工作区。当我们用HEAD时，表示最新的版本。

git rm {文件名}: 删除文件

