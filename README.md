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