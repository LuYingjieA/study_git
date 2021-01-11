git本地仓库初始化与Github远程仓库

###### 1. 创建本地ssh key

```shell
ssh-keygen -t rsa -C '517655364@qq.com'
```

###### 2. 复制id_rsa.pub 中的key到Github中的SSH key

###### 3. 测试是否连通

```shell
ssh -T git@github.com
```

###### 4. 本地配置

```shell
git config --global user.name 'LuYingjieA'
git config --global user.email '517655364@qq.com'
```

###### 5. 创建本地文件夹并初始化git

```shell
mkdir study_git
git init
```

###### 6. 添加远程仓库连接

```sh
git remote add study_git https://github.com/LuYingjieA/study_git.git
```

###### 7. 拉取最新代码 main分支

```shell
git pull sytudy_git main
```

###### 8. 第一次修改并提交

```shell
git add *
git commit -m '第一次提交'
git push study_git main
```



