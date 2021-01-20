# git-

#### 向仓库中添加文件流程

- 工作区(Working Directory)-->暂存区  
  - ```git status 得到当前文件的状态```
  - ```git add xxx.xx``` 文件从工作区->暂存区
- 暂存区-->Git Repository(Git 仓库)
  -```git  status```
  - ```git commit -m 'xxxx' ``` 提交描述

#### Git初始化及仓库创建和操作

- 基本信息设置
  - 设置用户名 ```git config --global user.name 'xxx'```
  - 设置用户名邮箱 ```git config --global user.email 'xxxx'```
- ```mkdir test``` 新建一个文件夹 
- ```cd test```进入
- ```git init```初始化
- ```touch a.js``` 新建文件
- ```git add a.js``` 添加到暂存区
- ```git commit -m 'add js'``` 添加到仓库
- 修改文件，修改后重复上面步骤
- 删除文件
  - ```rm a1.js``` 
  - ```git rm a1.js``` 从git中删除文件
  - ```git commit -m 'xxx'```

#### 管理远程仓库

- git克隆操作
  - git clone 仓库地址

#### 将本地已有项目上传到github

- 连接 ```git remote add origin 'xxxx'```
- 上传 ```git push -u origin master```

#### 个人站点 http://xx.github.io

- 仅支持静态网页，仓库里面只能是html文件

#### 删除文件夹下的所有 .git 文件

- ```find . -name ".git" | xargs rm -Rf```

#### 打标签

- ```cpp
  git tag -a 0.1.3 -m “Release version 0.1.3 
  git tag 是命令 -a 0.1.3是增加 名为0.1.3的标签-m 后面跟着的是标签的注释
  ```

- 分享提交标签到远程服务器上

  ```cpp
  git push origin master
  git push origin --tags
  –tags参数表示提交所有tag至服务器端，普通的git push origin master操作不会推送标签到服务器端。
  ```

- 切换到已有Tag

  ```cpp
  git tag --list  // 查看已有tag列表
  git checkout [tag/branch/commit]  // 切换到指定tag/branch/commit都是此命令
  ```

- 删除标签的命令

  ```cpp
  git tag -d 0.1.3
  ```

- 删除远端服务器的标签

  ```cpp
  git push origin :refs/tags/0.1.3
  ```
#### 创建一个分支并切换
```git checkout -b A //创建一个名为A的分支```
  
