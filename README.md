# windows-mysql

### 第一步 下载mysql
```markdown
  1. 下载地址：https://dev.mysql.com/downloads/mysql/
  2. 解压到相应的文件夹下
  3. 将mysql添加到环境变量
```

### 第二步 安装mysql
```markdown
  1. 生成data文件 cd到mysql下的bin目录 执行 mysqld --initialize --user=mysql --console 将生成的密码保存
  2. 安装mysql 以管理员权限打开cmd 执行 mysqld -install 
  3. 启动服务 net start MySQL
```

### 第三步 修改账号密码
```markdown
  1. 登录 mysql 执行 mysql -u root -p （输入保存的原始密码）
  2. 修改初始密码 ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY '*********';
  3. 保存设置 flush privileges;
  4. 退出 quit;
```
