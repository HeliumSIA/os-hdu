#### 题目
利用 linux 的共享内存通信机制实现两个进程间的通信:
编写程序 sender，它创建一个共享内存，然后等待用户通过终端输入一串字符，并将这串字符通过共享内存发送
给 receiver;最后，它等待 receiver 的应答，收到应答消息后，将 接收到的应答信息显示在终端屏幕上，
删除共享内存，结束程序的运行。编写 receiver 程序， 它通过共享内存接收来自 sender 的消息，将消息显
示在终端屏幕上，然后再通过该共享内 存向 sender 发送一个应答消息“over”，结束程序的运行。使用有名信
号量或 System V 信号 量实现两个进程对共享内存的互斥及同步使用。

#### 使用

```shell
make sender
make receiver

#
./sender
./receiver
```