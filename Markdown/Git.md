# Git

## 一、基础操作

### 1. 新建仓库

	git init

### 2. 增加临时文件

	git add .

### 3. 本地仓库更新

	git commit -m ""

### 4. 本地关联远程仓库

	git remote add (标识名(origin))  (远程地址)

### 5. 将本地仓库内容上传到远程仓库

	git push (标识名)(本地)

## 二、多人开发

### 1. 将远程仓库复制到本地，并自动形成本地仓库（仅用于第一次，其他时候使用pull）

	git clone (远程地址)

### 2. 将本地仓库内容上传到远程仓库

	git push (标识名)(本地)

### 3. 从远程仓库下载内容到本地仓库

	git pull (标识名) (本地)
	备注（需要基本操作中的命令）

## 三、分支

### 1. 查看当前仓库分支

	git branch
	仓库中默认只有master 分支
	执行 git commit 时，默认是在master 分支上保存版本

### 2. 创建分支

	git branch (分支名称)
	master 分支 不要轻易使用（较为稳定的版本存于master）
	开发时 创建开发分支

### 3. 切换分支

	git checkout (分支名)


![git](https://gitee.com/code-shuai/map-depot/raw/master/Git/git.png)

