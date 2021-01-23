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

创建分支，

合并分支（如果是master 需要合并demo-1,需要先保证已切换到了master），

再推送到远程

使用git pull 时需注意  这里的是修改的同个文件的情况（

本地没有提交的才能成功，否则会git pull失败，验证得出的

如果删除内容再强制推送会导致别人修改的文件掉失 let pull1 = pull1 不见了

） 