## Learngit 学习笔记
#### 1.Linux上安装Git
    sudo apt-get install git
#### 2.配置git
    git config --global user.name "Your Name"
    git config --global user.email "email@example.com"
    添加ssh公钥
    ssh-keygen -t rsa -C "pengshp3@outlook.com"
    cd  ~/.ssh
    cat id_rsa.pub
#### 3.创建版本库
    mkdir learngit
    cd learngit
    git init
#### 4.添加文件到版本库
    git add readme.txt
    git commit -m "wrote a readme file"
#### 5.查看版库信息
    git status
    git diff
#### 6.添加版本库,使与本地库关联
    git remote add origin git@github.com:pengshp/learngit.git
#### 7.把本地库的所有内容推送到远程库上
    git push -u origin master             (first)
    git push origin master
#### 8.从远程库克隆一个库到本地
    git clone git@github.com:pengshp/mylinux.git
#### 9.让Git显示颜色
    git config --global color.ui true
#### 10.忽略特殊文件
    在Git工作区的根目录下创建一个特殊的.gitignore文件，然后把要忽略的文件名填进去.
    eg.  *.py[cod]
         *.so
         *.egg
         *.egg-info
#### 11.配置别名
    git config --global alias.st status
#### 12.创建分支
    git checkout -b <name>
#### 13.切换分支
    git checkout master
#### 14.合并分支
    git merge <name>
#### 15.列出Git设置
    git config --list
#### 常用配置：
* 避免PULLING提交合并   
    git config --global branch.autosetuprebase always
* 颜色高亮:

    git config --global color.ui true
    git config --global color.status auto
    git config --global color.branch auto

 * 显示中文
 
    git config --global core.quotepath false # 设置显示中文文件名

##### Visual Studio2017上使用GitHub
#### [https://visualstudio.github.com/](https://visualstudio.github.com/)

##### *备注*：默认的配置都在`~/.gitconfig `文件夹下，这里列出了一些我认为经常用到的命令，记录自己的学习，也方便查看！！
##### 参考学习：[http://www.liaoxuefeng.com/](http://www.liaoxuefeng.com/)
##### [https://github.com/pengshp/](https://github.com/pengshp/)
