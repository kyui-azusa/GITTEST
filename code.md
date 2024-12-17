## 配置

### 1. 远程仓库

1. 创建SSH Key：

    ```bash
    $ ssh-keygen -t rsa -C "youremail@example.com"
    ```
    
    一路回车即可
    
    - `id_rsa`是私钥, 不能泄露.
    
    - `id_rsa.pub`是公钥, 可以告知他人.  
    
2. 查看`SSH Key`

    ```bash
    $ cd ~/.ssh
    $ cat id_rsa.pub
    ```

    也可在用户主文件夹下`./.ssh`目录查看

3. 配置`SSH Key`

    在`Github`的用户`Setting`选择`New SSH Key`, 起任意`Title`, 粘贴公钥.

### 2. 本地仓库

1. 初始化仓库

    ```bash
    $ git init
    ```

    目录下会生成名为的`.git`文件夹

2. 将本地仓库和GitHub仓库关联

    ```bash
    $ git remote add origin <仓库URL>
    ```

    origin为设置的别名

    项目url为: `git@github.com:kyui-azusa/GITTEST.git`
    
    * 修改`origin`
    
        ```bash
        $ git remote set-url origin <新的URL>
        ```
    
    * 删除`origin`
    
        ```bash
        $ git remote remove origin
        ```

## 使用

### 3. 提交版本(本地)

1. 把待提交文件添加到操作区

    ```bash
    $ git add <文件名/路径>
	```
	
	可用 `.` 代表所有文件, 多个文件可用空格分割

2. 提交修改

    ```bash
    $ git commit -m <message>
    ```

    - `-m` 后的参数为本次提交的说明
    - 一次`commit`可多次`add`不同的文件

### 4. 提交本地代码到github

1. 首次推送

    ```bash
    $ git push -u origin master
    ```

    首次推送，需要使用”-u”参数来设置默认的上游分支为`master`

    我们第一次推送`master`分支时，加上了`-u`参数，Git不但会把本地的`master`分支内容推送的远程新的`master`分支，还会把本地的`master`分支和远程的`master`分支关联起来，在以后的推送或者拉取时就可以简化命令
    
2. 简化

    ```bash
    $ git push origin master
    ```


## 吐槽

狗屎 一直fatal 研究了好久发现就两个问题

1. url输错了

2. origin输成origin 又不稳定错

    气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了气死我了