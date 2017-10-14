版本控制器：
    git和svn的区别：
	svn：集中式
	git：分布式

识别用户名和密码：
$ git config --global user.name "Your Name"
$ git config --global user.email "email@example.com"

通过 git init 命令把当前的目录变成一个仓库

注意：dir修改为ls  使用ls -ah可以查看隐藏文件

版本库添加文件：
   git add filename
版本库提交文件
   git commit -m ‘备注’
查看版本库状态：
   git status
查看文件的修改： 需要文件没有被添加和提交才可以查看
   git diff
查看历史版本
   git log 
   简化输出信息：git log --pretty=oneline
回退或回到某个版本
   git reset --hard HEAD^ (版本代码)

工作区和暂存区：
    工作区：当前正在编写代码的区域
    暂存区：通过git add提交的区域

管理修改：
    如果遇到刚刚所述问题：
        1.每次修改完记得add
        2.不管什么时候，全部add在提交

撤销修改：
     git checkout -- filename

git和github的关系：github使用git作为唯一代码托管方案

创建与合并分支：
    查看分支：git branch
    创建分支：git branch <name>
    切换分支：git checkout <name>
    创建+切换分支：git checkout -b <name>
    合并某分支到当前分支：git merge <name>
    删除分支：git branch -d <name>

冲突：手动修改文件


关联github：
    1.关联github：git remote add origin git@github.com:Geekiwen/hello.git
    2.将本地版本库推送到服务器上：git push -u origin master

克隆：git clone url

gitoschina:pull：下载