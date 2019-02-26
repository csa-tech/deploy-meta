将这个repository clone到本地，修改deploy-meta.json，再push就行啦。

deploy-meta.json的写法参考已有的例子：

- pusher: 你的GitHub账号
- repo: Repository name
- branch: 你想构建的branch
- port: 3010~3100中的任意一个数字。不要和别的小伙伴相同就行

push之前务必注意检查格式

两条设置，不可以pusher和repo都相同
（也就是说每个pusher在每个repo里可以填写至多一个branch）