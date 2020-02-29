# 1. 安装 samba

```shell
sudo apt install samba
```

# 2. 修改配置文件，增加共享路径

```shell
# 配置文件路径
/etc/samba/smb.conf

# 增加共享路径
sudo vim /etc/samba/smb.conf

# 写入如下的共享路径
[work]
comment = ubuntu work dir
path = /home/jam/work
browseable = yes
writable = yes
```

# 3. 重启 samba 服务

```shell
service smbd restart
```

# 4. 增加访问的用户权限

```shell
# 增加访问的可以用户共享路径的用户，并设置密码
sudo smbpasswd -a jam
```

# 5. Todo

- [ ] 把该过程写成脚本，下次安装自动化
