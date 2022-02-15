git 的学习
cat 文件名: 查看文件
git add:  文件名暂存 
git commit -m 本次提交的说明 : 提交
git log: 显示从最近到最远的提交日志
git log --pretty=oneline: --pretty=oneline(嫌输出信息太多，看得眼花缭乱的，可以加上--pretty=oneline参数)
git reset --hard HEAD^ : 回退到上一个版本就是HEAD^(HEAD指向的版本就是当前版本)
git reset --hard HEAD^^ : 回退到上上一个版本就是HEAD^^
git reset --hard {commit id} : 可以指定回到未来的某个版本
git reflog: 用来记录你的每一次命令
