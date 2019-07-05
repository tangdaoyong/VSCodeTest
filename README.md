# VSCodeTest
visual Studio Code git test(使用测试)

VSCode 使用git进行版本管理，测试demo。

## 添加本地忽略文件.gitignore

[.gitignore忽略规则的匹配语法参考](https://www.cnblogs.com/kevingrace/p/5690241.html)
[github中gitignore模板](https://github.com/github/gitignore)

### 在github上创建工程的时候可以勾选.gitignore

### 手动创建

1. 进入工程目录，.git相同目录下。**touch .gitignore**命令创建文件
2. **vim .gitignore**编辑文件。
3. **git rm -r --cached .** 删除本地缓存（需要忽略的文件已经push了）
> 如果是文件夹：git rm -r --cached 文件夹名
> 如果是文件：git rm --cached 文件名
3. **git reset <commit_id>**这个命令, 把 commit 历史撤销，对应缓存区内容也撤销，工作区内容不变(已经 commit 提交了，但是还没有 push 到远程)
4. **git add .** 添加要提交的文件
5. **git commit -m '提交说明'**更新本地的缓存