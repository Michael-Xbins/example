	A，B 两个进程通过管道通信，像以前的互相聊天一样，然后A 进程每次接收到的数据通过A1 进程显
示（一个新进程，用于显示A 接收到的信息），A 和A1 间的数据传递采用共享内存，对应的有一个B1
进程，用于显示B 进程接收到的信息。针对A，B 进程，退出时采用ctrl+c 退出，当收到对应信号后，
自身进程能够通过信号处理函数进行资源清理，清理后exit 退出进程。（A1，B1，手动关闭即可）。界
面图如下。

