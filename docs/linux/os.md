# Linux

系统

---

## 系统安装（Arch Linux）

## 配置

### 用户

```sh
# 增加用户
useradd test
passwd test
chsh -s /usr/bin/fish

# ssh
ssh-keygen -t rsa
ssh b@B mkdir -p .ssh
cat .ssh/id_rsa.pub | ssh b@B 'cat >> .ssh/authorized_keys'
ssh b@B

# /etc/ssh/sshd_config
# Port 22 -> Port xxxx  (xxxx > 1024)
service sshd restart
```

### 常用软件

#### VIM

```sh
# CentOS 7
sudo yum install vim
```

#### zsh

```
# antigen-hs
cabal install base text directory filepath process
git clone https://github.com/Tarrasch/antigen-hs.git ~/.zsh/antigen-hs/
antigen-hs-compile  # after update MyAntigen.hs
```

#### fish

```sh
# CentOS 7
cd /etc/yum.repos.d/
wget http://download.opensuse.org/repositories/shells:fish:release:2/CentOS_7/shells:fish:release:2.repo
yum install fish

# Arch Linux
pacin autojump
```

#### git

```sh
yum install git
```

#### shadowsocks

```sh
yum install python-setuptools && easy_install pip
pip install shadowsocks

ssserver -c config.json
# 后台
ssserver -c config.json -d start
ssserver -c config.json -d stop
```

## 常用命令

### 远程管理

```sh
# 复制
scp foobar.txt your_username@remotehost:/some/remote/directory
```

### 字数统计

```sh
texcount FILE
```
