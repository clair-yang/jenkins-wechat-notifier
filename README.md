# jenkins-wechat-notifier
Jenkins微信通知插件

微信通知插件用于在构建完成后通过企业微信应用向指定用户或群聊发送消息通知

增加pipeline支持
```
step(
  [$class: 'WechatNotifier',
   successMsgType: [$class: 'Text', content: '测试消息，请忽略。构建成功'],
   disablePublish: false,
   receivers: [[type: 'user',id: 'YangPengHui']],
   failMsgType: [$class: 'Text', content: '测试消息，请忽略。构建失败']]
)
```
