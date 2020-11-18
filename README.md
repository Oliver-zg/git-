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
- git remote add origin 'xxxx'
#### 个人站点 http://xx.github.io
- 仅支持静态网页，仓库里面只能是html文件
