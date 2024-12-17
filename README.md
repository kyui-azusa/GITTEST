# git命令

> author: zzy

## 标注说明

*步骤表示非必须, 辅助用.

## 本地项目

### 初始化项目

1. - **新建文件夹**
	
        ```bash
        mkdir <foldername>
        ```
	     
    -  **将工作目录跳转到新建的文件夹**
       
        ```bash
      cd <foldername>
      ```
      或

    - **直接在已有工作目录下打开git终端**

2. ***显示当前目录**

	
    ```bash
    pwd
    ```
    
3. **把这个目录变成Git可以管理的仓库**
   
    ```bash
    git init
    ```

### 把文件提交到版本库(提交修改为新版本)
1. **将文件添加到操作区**
   
    ```bash
    git add <filename>
    ```
    - 执行后无提示


2. **提交修改**
   
    ```bash
    git commit -m <message>
	```
    - `-m` 后的参数为本次提交的说明
    - 一次`commit`可多次`add`不同的文件:
    ```bash
    $ git add <file1>
    $ git add <file2> <file>
    $ git commit -m "add 3 files"
    ```
```bash
git status
```


```bash
git diff
```

```bash
git log
git log --pretty=oneline
```

```bash
git reset --hard <id>
git reset --soft <id>
git reset --mixed <id>
# id: HEAD: 当前版本 HEAD^: 上个版本 HEAD~100: 上100个版本
```

```bash
git reflog
```

```bash
cat <filename>
```

```bash
git diff HEAD -- <filename>
```

```bash
git restore
```

```bash
rm <filename>
git add <filename>
# =>
git rm <filename>
```

