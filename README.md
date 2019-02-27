**Step 1: 在自己的repository里设置webhook**

在GitHub打开这个repository的界面，点击上方靠右边的[Settings] tab （在[Watch]下方）

点击左侧 [Webhooks]

右边点 [Add webhook]，

Payload URL 填 http://13.56.241.40:8082/webhook/

Content type 选 application/json

Secret 不用管

Which event... 只选第一个 just the push event

Active 选中

最后点绿色 [Add Webhook]


**Step 2: 在这个repository**

将这个repository clone到本地，修改deploy-meta.json，再push就行啦。

deploy-meta.json的写法参考已有的例子：

- pusher: 你的GitHub账号
- repo: Repository name
- branch: 你想构建的branch
- port: 3010~3100中的任意一个数字。不要和别的小伙伴相同就行

**注意！！！！！**

push之前务必注意检查格式

两条设置中，不可以pusher和repo都相同
（也就是说每个pusher在每个repo里可以填写至多一个branch）