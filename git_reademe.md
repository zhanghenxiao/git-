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