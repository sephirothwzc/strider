# 步骤

```s
# 下载
$ git clone https://github.com/Strider-CD/strider.git && cd strider
$ rush install
# install 报错，修改 apidoc-markdown: 5.2.5
$ cd apps/strider
# 创建登陆用户
$ node bin/strider addUser
# 用户名、密码、是否admin
# 插件安装 gitlab
$ bin/strider install gitlab
# 启动
$ npm start
```

- mongodb

```mongodb
>use admin
>db.auth('用户名','密码')

>use strider
>db.createUser({user: "strider", pwd: "striderpw", roles: [{role: "dbOwner",db:"strider"}]})
```
