# SSH

ssh 的基本使用形式：

```
ssh 用户@主机
```

用户是你登录服务器用的用户名，@ 符号右边是服务器的主机名或者 IP 地址。

比如我要连接之前创建的 CentOS 系统的虚拟机，这台机器有个 IP 地址是 192.168.33.20，连接到它可以这样：

```
ssh vagrant@192.168.33.20
```

vagrant 是我连接服务器的时候使用的用户，这个用户应该提前在服务器上创建好。服务器一开始一般只有一个超级管理员叫 root，第一次登录到服务器，通常你就需要使用 root 身份登录。

第一次连接到某台服务器，可能会出现这样的提示：

```
The authenticity of host '192.168.33.20 (192.168.33.20)' can't be established.
ECDSA key fingerprint is SHA256:YdSnCe4b5efT7xy5pOX4lG/dJBPVVBNHaj7RR1cAm5o.
Are you sure you want to continue connecting (yes/no)?
```

输入 yes ，然后回车。可能会提示你输入跟 vagrant 用户对应的密码，也可能会提示：

```
Permission denied (publickey,gssapi-keyex,gssapi-with-mic).
```


