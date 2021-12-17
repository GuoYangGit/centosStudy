# Linux 常用命令

## 软件操作命令

|命令|说明|
|:--:|:--:|
|yum install xxx|安装软件|
|yum remove xxx|卸载软件|
|yum search xxx|搜索软件|
|yum clean packages|清理缓存|
|yum list|列出已安装软件|
|yum info xxx|软件包信息|

## Linux文件目录结构

> 根目录 /  
> 用户目录 /home  
> 临时目录 /tmp  
> 配置目录 /etc  
> 用户程序目录 /usr  

## 文件操作命令

|命令|说明|
|:--:|:--:|
|ls|查看目录下的文件|
|touch 文件名|创建文件|
|mkidr 文件夹名|创建文件夹|
|cd 目录路径|进入目录|
|cat 文件名|查看文件|
|rm 文件名|删除文件和目录|
|cp 来源 目标|复制文件|
|mv 来源 目标|移动文件|
|pwd|显示路径|
|wget 下载地址|下载文件|
|curl -o 本地保存命名 下载地址|下载文件|
|scp 本地文件 远程服务器存放路径|上传文件|


## vim常用命令

|命令|说明|
|:--:|:--:|
|i|编辑模式|
|esc|退出编辑模式|
|:q|退出|
|:qw|退出并保存|

## 系统用户操作命令

|命令|说明|
|:--:|:--:|
|useradd|添加用户|
|adduser|添加用户|
|userdel|删除用户|
|passwd 用户名|设置密码|
|visudo||

## 用户提权操作

```
# 输入指令
visudo

# 找到## Allows people in group wheel to run all commands
# 添加用户 %guoyang ALL=(ALL)       ALL
```