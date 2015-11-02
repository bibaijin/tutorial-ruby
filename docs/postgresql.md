# PostgreSQL

数据库

---

## 安装

```sh
sudo pacman -S postgresql
```

## 配置

```sh
sudo -i -u postgres
initdb --locale en_US.UTF-8 -E UTF8 -D '/var/lib/postgres/data'
systemctl start postgresql.service
systemctl enable postgresql.service
createuser --interactive
createdb test
```
