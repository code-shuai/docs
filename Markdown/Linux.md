# Linux









## 基本操作

### 命令 - 目录

#### `pwd`   

	显示当前目录的绝对路径
	绝对路径：从根目录起始的路径
	相对路径：从指定路径起始的路径

#### `cd`   

	切换目录
	返回至当前用户起始目录 `cd` or `cd ~`

#### `mkdir`   

	创建文件夹
	
	`mkdir -p [directory name]`
	创建多级目录

#### `rmdir`   

	删除目录（只能删除空目录）
	
	`rmdir -p [directory name]`
	递归删除目录
	
	`rm -r dir`
	删除非空目录

#### `ls`   

	列出目录下文件清单
	
	`ls -a`
	显示所有子目录和文件，包括隐藏文件
	
	`ls -l`
	以长格式显示文件的详细信息
	
	`ls -t`
	按修改时间排序
	
	`ls -r`
	递归的显示各个子目录中的文件

### 命令 - 文件

#### `cat`   

	查看、创建、合并文件


### 命令 - 其他

#### `tar`   

#### `grep`   

#### `awk`   





# Ubuntu



### 环境配置



- dotnet core sdk
- git
- nginx
- nodejs
- npm
- cnpm
- vue
- 



### nginx



服务



查看状态

````
systemctl status u-mvc-app.service
````

停止

```
systemctl stop u-mvc-app.service
```

开启

```
systemctl start u-mvc-app.service
```







### desktop



```
 apt-get update   //更新软件库
 apt-get upgrade   //升级软件
 apt-get install ubuntu-desktop    //安装Ubuntu桌面系
```



### root 登录





### vs code



```
sudo snap install --classic vscode
```

新

```
sudo snap install code --classic
```





