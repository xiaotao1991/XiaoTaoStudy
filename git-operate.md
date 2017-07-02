## git学习 ##

初始化仓库

    git init

文件添加到仓库 
  
    git add file1 file2


文件 提交
    
    git commit -m "描述"

查看命令结果

     git status

比对修改了什么内容

    git diff

版本回退
    
	git reset --hard HEAD^   	回退到上一个版本
	git reset --hard HEAD~100   回退到指定版本

查看提交历史
  
	git log			以便确定要回退到那个版本

查看命令历史

	git reflog 		以便确定要回到未来的那个版本

暂存区
	
	提交文件 1.先add文件到暂存区
			2.在commit，实际上是把暂存区的所有内容提交到当前分支

在还没有提交时，或是add到暂存区中。让当前文件回到最近一次commit
	
	git checkout --file

删除文件
	
	git rm file
    git commit -m "删除文件"

如果文件错删了
	
	git checkout --file    可以把误删的文件恢复到最新版本

关联一个远程库
	
	git remote add origin git@server-name:path/repo-name.git

提交分支上修改的内容
	
	git push -u origin master 	第一次推送master分支的所有内容
	git push origin master		推送最新的修改

clone远程仓库
	
	git clone git@github.com:xiaotao1991/gitskill.git


创建分支
	
	git checkout -b dev
	等同于命令:
	git branch dev
	git checkout dev

查看当前分支
	
	git branch 

合并到主分支
	
	git merge dev

删除分支
	
	git branch -d dev
	git branch -D dev 	强行删除分支

冲突解决

	手动删除冲突 <<<<<<< , ======= ,>>>>>>>>

bug分支，需要尽快的修复bug，但正在开发的代码还未提交
	
	git stash 		可以把工作现场“存储”起来，等恢复现场后继续工作
	git stash pop 	把stash存储的内容恢复，同时把stash的内容也删除了

Feature分支  新功能的添加，又不想把主分支搞乱
	

推送分支

	git	push origin master
	git push origin dev

同步分支
	
	git pull 
	git branch --set-upstream dev origin/dev 指定本地的dev分支与远程的origin连接

