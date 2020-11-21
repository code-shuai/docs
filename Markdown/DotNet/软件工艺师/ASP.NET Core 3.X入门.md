## 1. 创建项目

### 包管理

- 服务器端（后端）：Nuget
- 前端：Npm（Node Package Manager）/ 客户端库


	Npm：新建 package.json 文件
	客户端库：libman.json
	打包：
		创建 bundleconfig.json 
		nuget 添加 BuildBundlerMinifier
		重新生成解决方案时会自动打包




## 4. 配置信息


### 配置信息介绍

- Key-Value
- 内存、JSON、XML、INI、系统环境变量
- 配置信息与配置系统解耦
- 依赖注入

```
上文解释：

1. 配置信息是以键值对的形式存在的
如：数据库连接字符串
2. 配置信息一般可以存入内存里、JSON 、XML 、INI 等文件中，或者系统环境变量中
3. 配置信息与配置系统解耦：配置信息可以在项目中任何地方使用
4. 通过依赖注入使用配置信息从而达到任何地方可使用
```

### 配置信息来源

```
第一会找
  .net core 运行的时候，它会找一个叫 appsettings.json 的文件
  然后会根据环境（开发环境、生产环境）找 appsettings.[environment].json 的文件 
第二会找
  Secret Manager 
  如果与上面文件信息有相同，则会使用此文件中信息
第三会找
  环境变量中
第四会找
  命令行参数


```




