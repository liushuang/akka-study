# akka-study

# actor 模型
* 一个Actor是一个最基本的计算单元，他接收一个消息并执行对应的计算。
* 每一个actor有自己的地址
* 每个actor只能顺序的处理一条消息
## actors有邮箱（Mailbox）
消息异步地传送到actor，所以当actor正在处理消息时，新来的消息应该存储在别的地方，Mailbox就是这些消息存储的地方。

## Actors做什么
当一个actor接收消息后，他做如下三件事中的一件：
1. 创建其他actor
2. 向其他actors发送消息
3. 指定下一条消息到来的行为

## 随他崩溃


