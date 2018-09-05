this is a readme txt!
git is a version contral system
this is my first time use git


1,git init   //用于初始化Git库
2,git add xxx.txt   //向库中添加文件    把文件修改添加到暂存区
3,git commit -m "xxxx"   //提交对这次修改的记录  把暂存区的所有内容提交到当前分支   每次修改，如果不用git add到暂存区，那就不会加入到commit中。
4,git status  //查看库中文件的状态
5,git diff   //查看修改前后文件的异同
6,git log     //查看修改时提交的文件commit
7,git reset --hard HEAD~x           //返回到之前某一版本，当前版本为HEAD~0  往前以此类推
  git reset --hard commit id     //穿梭到某一版本，只需输入版本号的前几位    git reset命令既可以回退版本，也可以把暂存区的修改回退到工作区
8,git reflog    //查看之前的操作日志
9,git checkout -- xxx.txt   //意思就是，把readme.txt文件在工作区的修改全部撤销，这里有两种情况：
                            一种是readme.txt自修改后还没有被放到暂存区，现在，撤销修改就回到和版本库一模一样的状态；
							一种是readme.txt已经添加到暂存区后，又作了修改，现在，撤销修改就回到添加到暂存区后的状态。
10,git rm xx.txt    //从库中删除某一文件，该操作只删除该文件最新版本，之前的版本可以通过git reset回退找回