# 生成rsa文件
> 在.ssh文件夹下生成
``` sh

$ ssh-keygen -t rsa -C "youremail@example.com"

```

# 连接远程git仓库
$ git remote add origin git@github.com:michaelliao/learngit.git

# 推送本地仓库到github
$ git push -u origin master

# 拉取github数据到本地仓库
$ git pull origin master

# 从远程仓库上克隆数据到本地
$ git clone git@github.com:nixiaohui/gitskills.git


# 创建一个分支仓库dev，并切换到该分支
$ git checkout -b dev
Switched to a new branch 'dev'

# 以上命令，等于以下两行命令
$ git branch dev
$ git checkout dev
Switched to branch 'dev'

# 查看分支
$ git branch
* dev
  master

# 切换分支
$ git checkout master
Switched to branch 'master'

# 合并dev分支到master下
$ git merge dev
Updating d46f35e..b17d20e
Fast-forward
 readme.txt | 1 +
  1 file changed, 1 insertion(+)


