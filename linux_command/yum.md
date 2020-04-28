## yum 基本使用

### yum 的介绍
`yum` 软件包管理器，可以理解为是一个软件的仓库，方便进行依赖环境的安装，与 `apt-get` 和 `brew`(Mac平台) 具有相同的功能。

### yum 的安装
centos 系统默认安装


### yum 的使用
*需要root权限*

1. 查找指定软件包
`yum search xxxx` 
以名字为关键字
`yum provides xxxx` 
以提供的信息为关键字

2. 安装指定软件包  
`yum install xxxx`

3. 删除指定软件包  
`yum remove xxxx`

4. 列出所有已安装的软件包  
`yum list installed`

5. 升级指定软件包  
`yum update xxxx`

6. 清除缓存目录(/var/cache/yum)  
`yum clean packages/headers/oldheaders`

7. 查看软件信息
`yum info xxxx`

- -y 参数  指定安装过程中的yes

==思考==: 怎么安装redis mysql nginx等常用工具，源码？命令行？

*源码安装*：官网或github下载源码，可选择版本，支持定制化编译模块，适合深度开发和特殊需求
*命令行安装*：安装简单，适合初步入门学习使用

==遗留==：
- wget的使用
wget就是一个下载器，可以下载参数对应的地址
- markdown 的画图相关的高级语法
需要安装高级插件，后面有时间可以进行尝试
- vim 高级插件的安装
需要安装高级插件，后面有时间可以进行尝试


