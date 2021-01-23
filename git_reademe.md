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