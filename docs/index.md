# 认识SSH

## 安装SSH

```
yum install openssh-server
```

## 启动SSH

```
# 启动sshd服务
service sshd start

# 重启sshd服务
service sshd restart

# 停止sshd服务
service sshd stop
```

## 设置开机运行

```
chkconfig sshd on
```

## 查看进程命令

```
ps -ef |grep ssh
```

## 连接远程服务器

```
ssh 用户名@远程服务器IP地址
```

## 退出远程服务器

```
exit
```

## SSH config命令

> 文件存放地址: 本地(~/.ssh/config)文件

```
Host "远程服务器连接命名"
    Hostname 远程服务器IP地址
    User 用户名
    Port 端口号(默认端口都是22)
    IdentityFile SSH公钥存储路径
    IdentitiesOnly yes(是否使用RSA方式登录)
```

## 生成SSH Key

```
ssh-keygen -t rsa
```

## 远程服务器存放公钥

> 文件路径 ~/.ssh/cat authorized_keys
```
# 编辑该文件
vim ~/.ssh/cat authorized_keys

# 将生成的公钥填充在这个文件里面
```

## 修改SSH服务端口

> 文件路径 /etc/ssh/sshd_config
> 修改文件中Port的值(默认22端口)