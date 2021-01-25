##### 生成公钥和私钥

用ssh 生成的公钥和私钥  rsa不对称的加密方式

```
ssh-keygen -t rsa -C 'cookie.com'
```

  windows 默认生成的位置C:\Users\RE\.ssh  带pub的是公钥我们需要copy到gitbub 上

注意我们clone  仓库要使用ssh 的url   公钥才会生效



##### vscode 使用git

commit  信息一定要清晰，有几条就列几条

插件 git history diff

1.创建分支，

2.合并分支（如果是master 需要合并demo-1,需要先保证已切换到了master），

3.再推送到远程

4.使用git pull 时需注意  这里的是修改的同个文件b.js的情况（

本地b.js修改了还没有，使用git pull失败，验证得出的

如果本地b.js删除未提交内容 再强制推送 会导致远程别人修改的b.js 掉失 let pull1 = pull1 不见了



若 本地有c.js的文件未提交，我们使用git pull 能正常拉取数据到本地

##### 使用git pull 最好建议

最好的建议就是先保证本地工作区是干净的，我们再使用git pull，因为我们也不知道那些人到底改了那个文件 

） 

##### git 命令行

vim 一些常用命令



查看本地分支 git branch 

查看本地和远程分支 git branch -a

创建本地分支(git branch demo-2)，推送分支到远程(git push origin demo-2 )

删除本地分支(git branch -D demo-2), 删除远程分支 （git push origin --delete demo-2）

提交信息  git commit -m '使用-a 没有被add 暂存的也能提交'  -a



tag 是我们上线后，一个操作，分支的是v1.0.0,标签是t1.0.0这是规范

查看所有tag   git tag --list

创建本地tag 处于当前需要创建的位置  (git tag t1.0.0) ，tag推送到远程 git push origin t1.0.0

删除本地tag  (git tag -d t1.0.0), 删除远程tag (git push origin :t1.0.0)



回到文件未修改时的状态 git checkout .

版本回退revert

git revert e111(注意e111我们需要回退的版本，然后我们再推送)

git push origin demo-3 

版本回退reset，甚至干掉了历史记录，但是会导致冲突  我们强制推送下就可以了
