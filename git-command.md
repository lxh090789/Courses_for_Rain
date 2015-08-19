# git 命令

> 安装完成之后第一步是配置邮箱和姓名
> <Code>
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
  </Code>


>git init 在当前目录初始化一个版本库 （repository）

>git 只能跟踪文本文件的变动，其他2进制文件无法跟踪（比如ppt,execl等）

>git status 查看文件的跟踪情况

>git add fileName  把需要提交的文件添加到索引区
>git add . 
>git add *    添加所有变动的文件


>git commit -m "提交信息"  把当前索引区内的文件提交，并标注提交信息


>git log 查看提交的记录
>git log fileName 查看该文件的提交记录
>git log --pretty=oneline 、


>git reset --hard HEAD^
>HEAD表示当前提交 HEAD^ 表示上次提交  HEAD^^标识前两次提交 同理类推
>HEAD~100 表示前100次的提交

>git reset --hard HEAD^回退到上次提交
>git reset --hard 具体的提交号   ，git log 可查看版本号


>git reflog

>git rm fileName 删除文件





>ssh-keygen -t rsa -C "youremail@example.com"
一路回车，使用默认值即可
在用户主目录里找到.ssh目录，里面有id_rsa和id_rsa.pub两个文件，这两个就是SSH Key的秘钥对，id_rsa是私钥，不能泄露出去，id_rsa.pub是公钥


登陆GitHub，打开“Account settings”，“SSH Keys”
点“Add SSH Key”，填上任意Title，在Key文本框里粘贴id_rsa.pub文件的内容





git remote add origin xxxxxxxxxxxxxx.git
为当前git库添加远程源 
添加后，远程库的名字就是origin，这是Git默认的叫法，也可以改成别的，但是origin这个名字一看就知道是远程库。


git push 推送当前的提交
=git push origin master 即默认推送的是origin 远程库上的 master分支

关联远程库之后第一次推送到远程库的时候 需要加上 -u 参数 
即 git push -u origin master

git push 推送
git pull 拉取更新

git clone xxxx.git 
从当前目录复制一份已有的 远程库

git checkout -- fileName 撤销该文件所做的更改 ，恢复到未提交前

以下命令属于进阶
===============
分支 branch
合并分支 merge branch
