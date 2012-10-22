一直用goagent来翻墙，最近一直不稳定，而我又是google的重度使用者，所以就开始想其他的解决办法。

我有VPS， 所以对与这个来说，最简单的方法是用ssh 隧道来实现。具体步骤如下

1.目前有很多的VPS,便宜的有[Burst net](https://service.burst.net/aff.php?aff=2002),最便宜的不到6美金. 速度快而稳定的有[Linode](http://www.linode.com/?r=d9ee76f48097286f4832d02e67930354125e9f7d),基本上所有的VPS都支持ssh登陆的。

2.在mac上运行下面命令

    ssh -D 7000 {your accout}@{your host}

这个步骤基本上你已经在你mac上建立7000端口上的ssh channel了

3.在你的浏览器上用Proxy Switch sharp， 设置Socket5代理: localhost  7000  **注意要选择Socket v5**

开始享受吧

