### 环境准备 ###

1. OS: Ubuntu 14.04 LTS
2. Python3 & pip
```
apt install python3
apt install python3-pip
```
3. mariadb
```
apt install mariadb-server
```
安装过程中，为root设置一个密码，例如“xxxxxx”
4. 连接到mariadb
```
mysql -u root -p
```
输入前面设置的mariadb密码，应该可以正常登录。
5.创建数据库
```
create database moker;
show databases;
use moker;
```
6.安装和运行mocker
```
pip install -e .
FLASK_APP=mocker flask run --host=0.0.0.0 --port=8282
```
