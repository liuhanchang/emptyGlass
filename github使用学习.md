#github使用学习.md
##1.在github上创建项目

##2.本地clone项目
参考文章：http://www.worldhello.net/gotgithub/03-project-hosting/010-new-project.html
 git clone git@github.com:liuhanchang/emptyGlass.git

 git add README.md
 git commit -m "README for this project."
 提示：
 fatal: not a git repository (or any of the parent directories): .git
原因：没有git init

git add README.md
fatal: pathspec 'README.md' did not match any files
git commit -m "README for this project."
On branch master

Initial commit

Untracked files:
        emptyGlass/

nothing added to commit but untracked files present
git push origin master
error: src refspec master does not match any
error: failed to push some refs to 'origin'
git add .
error: 'emptyGlass/' does not have a commit checked out
fatal: adding files failed
原因：当前目录不对,切换到当前项目目录下即可
cd emptyGlass/

git add README.md
git commit -m "README for this project."

 git push origin master

##3.本机第一次连github,通过ssh命令
*git config --global user.name "871458219@qq.com"
*git config --global user.email "871458219@qq.com"

*生成密钥：ssh-keygen -t rsa -C "871458219@qq.com"
*密钥路径：C:\Users\Administrator/.ssh/id_rsa.pub.

*将 SSH 私钥添加到 ssh-agent
ssh-add ~/.ssh/id_rsa

*将 SSH 密钥添加到 GitHub 帐户。