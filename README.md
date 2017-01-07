gitskills

git add JavaScript/test.js
git commit -m "提交"
//当前状态
git status
//不同
git diff JavaScript/test.js
//历史
git log
//简化
git log --pretty=oneline
//回退到上一个版本
git reset --hard HEAD^
//会退到某一个版本
git reset --hard 版本号
//后悔药
git reflog
//查看工作区和版本库里面最新版本的区别
git diff HEAD -- README.md
//丢弃工作区的修改
git checkout -- README.md
//把暂存区的修改撤销掉
git reset HEAD README.md
//删除文件
rm test.txt
//从版本库删除该文件
git rm README.md
//生成SSH KEY id_rsa是私钥 id_rsa.pub是公钥
ssh-keygen -t rsa -C "646133621@qq.com"
//已有的本地仓库与远程关联
git remote add origin git@github.com:QHChen96/gitskills.git
//推送
git push -u origin master
//强制推送
git push -f origin master
//本地作了提交，就可以通过命令
git push origin master
加上了-u参数，Git不但会把本地的master分支内容推送的远程新的master分支
git push -u origin master
//创建dev分支,并切换
git checkout -b dev
/*以上相当于
创建分支
git branch dev
切换分支
git checkout dev
*/
//查看当前分支
git branch
//合并分支
git merge dev
//删除分支
git branch -d dev
//git log 查看分支合并情况
git log --graph --pretty=oneline --abbrev-commit
//合并分支，禁用fast forward，Git就会在merge时生成一个新的commit
git merge --no-ff -m "merge with no-ff" dev
//把当前工作现场“储藏”，针对，与当前代码无关，要解决其他问题
git stash
//恢复
git stash apply
//恢复但会删除stash
git stash pop
//stash列表
git stash list
//多人协作
//查看远程库信息
git remote
//更详细
git remote -v
//推送
git push orgin master
//抓取
git clone




