## 配置

	``` 1. 初始化仓库

```bash
git init
```

目录下会生成名为的`.git`文件夹

### 2. 将本地仓库和GitHub仓库关联
```bash
git remote add origin <仓库URL>
```

origin为设置的别名

项目url为: https://github.com/kyui-azusa/GITTEST/

## 使用

### 3. 提交版本

1. 把待提交文件添加到操作区

    ```bash
    git add <文件名/路径>
	```
	
	可用 `.` 代表所有文件, 多个文件可用空格分割

2. 提交修改

    ```bash
    git commit -m <message>
    ```

    - `-m` 后的参数为本次提交的说明
    - 一次`commit`可多次`add`不同的文件: