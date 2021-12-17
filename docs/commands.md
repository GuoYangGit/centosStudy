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