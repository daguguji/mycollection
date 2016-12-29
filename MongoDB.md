[Windows 安装启动 参考](http://www.runoob.com/mongodb/mongodb-window-install.html)

以安装到 C:\ 为例

```
c:\>cd c:\

c:\>mkdir data

c:\>cd data

c:\data>mkdir db

c:\data>cd db

c:\data\db>

```

> 命令行下运行 MongoDB 服务器

```
mongod.exe --dbpath c:\data\db
```

[创建数据库](http://www.runoob.com/mongodb/mongodb-create-database.html)

`use DATEBAE_NAME`

> 实例
```
> use runoob
switched to db runoob
> db
runoob
> 
```

> 查看已有的数据库

`show dbs`

无数据的数据库不会展示

要显示它，我们需要向 runoob 数据库插入一些数据

```
> db.runoob.insert({"name":"菜鸟教程"})
WriteResult({ "nInserted" : 1 })
> show dbs
local   0.078GB
runoob  0.078GB
test    0.078GB
>
```