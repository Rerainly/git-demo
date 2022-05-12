初始化文件：git init
查看文件情况：git status
查看文件列表：ll
添加工作区文件：vim 文件名.后缀名
把工作区文件添加到缓存区：git add 文件
把缓存区文件删除：rm --cached 文件名

查看文件信息：cat 文件名

提交文件：git commit -m "注释信息" 文件名

查看版本：git reflog

查看详细版本：git log

穿越版本号，就是回到某个版本:git reset --hard 版本号



分支操作：1

创建分支：git branch 分支名

查看分支：git branch -v

切换分支：git checkout 分支名

合并分支：git merge 分支名  注意（是站在当前分支合并你想合并的分支）

合并分支之后还有两部操作：

1.git add 文件名

2.git commit -m '记录'  (注意这次不需要带文件名)





远程库链接

我的远程库git-demo链接： https://github.com/Rerainly/git-demo.git
如果链接太长记不住，可以创建别名：git remote add 别名 连接名
查询别名:git remote -v
将本地仓库推送到远程仓库：git push 别名|链接  分支


将远程数据库的文件拉取回来:git pull 别名|链接 分支 
（注意拉取动作会自动帮你保存在本地库，所以不用commit了）

克隆:git clone 链接
以下有两个注意点：
1：当你clone了代码时候，修改了里面的代码，想push时候，需要做以下步骤
（注意如果同一个电脑push，需要到电脑凭据把你的登入信息删除了）
2：别人要给你发邀请码，或者自己发邀请链接给别人，然后在自己登入的github页面粘贴这个链接，然后点accept，这样就可以push了。

将别人的代码插入到自己的仓库中进行修改代码，我们课直接点击github或者gitee 别人项目右上角的fork，这样就可以直接插到直接仓库里面了



