# Git 创建仓库 #
## git init ##
用来初始化一个Git仓库
执行完 git init后，Git仓库会.git目录，该目录包含了资源的所有元数据，其他的项目目录保持不变
## 使用方法 ##
    git init
    git init newrepo

参数说明：
newrepo ：指定目录； 空为当前目录
## 添加文件进行版本跟踪 ##
首先使用git add 命令 进行添加跟踪文件，然后提交

    git add *.py
    git add add readMe.md
    git commit -m '初始化项目版本'

:将当前目录下的所有.py文件放入版本管理
:将当前目录下的 readMe.md 文件放入版本管理
:提交（附带备注信息）


# git clone #
使用 git clone 从现有 Git 仓库中拷贝项目.

## 使用方法 ##
    git clone <repo>
    git clone <repo> <directory>
参数说明：
repo:Git 仓库。
directory:本地目录。

比如，要克隆 Django 代码仓库 hello，可以用下面的命令：

    $ git clone git://github.com/Django/hello.git
执行该命令后，会在当前目录下创建一个名为hello的目录，其中包含一个 .git 的目录，用于保存下载下来的所有版本记录。
如果要自己定义要新建的项目目录名称，可以在上面的命令末尾指定新的名字：

     $ git clone git://github.com/Django/hello.git myhello

## 几种效果等价的git clone写法： ##

    git clone http://github.com/Django/hello new
    git clone http://github.com/Django/hello.git new
    git clone git://github.com/Django/hello new
    git clone git://github.com/Django/hello.git new