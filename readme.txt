提交文档
git add  read.txt
git commit -m "version infomation"
查看所有版本文件
git log
退回到上有版本
git reset --hard HEAD^
退回到指定版本 
git reset --hard + 版本的commit id
查看git状态
git status
撤销命令
git checkout -- 文件名
管理分支 
git checkout 
删除文件
先删除文件 或者bash 使用rm 然后使用git rm 文件名
然后提交 git commit -m  “删除原因”

创建远程仓 
1 . 再github 上创建好远程仓库 完成后复制ssh 地址或者http地址
2 . 本地仓库中git bash中输入 git remote add origin xxxxxxxxxxx（远程仓库地址）
注：如果出现错误 检测地址，地址正确的话 使用命令 git remote rm origin 后再次连接远程仓
完成后 使用 git push -u origin master(可以是其他分支)

克隆远程仓 
使用 git clone xxxxxxx 地址

远程仓更新后同步到本地仓
1. 查看远程仓库  git remote -v
2. 获取远程仓库内容 git fetch origin master(远程分支):master（本地分支）
3. 比较内容   git diff master
4.合并分支 git merge master 

