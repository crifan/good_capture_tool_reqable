# 抓包和代理软件会冲突

使用Reqable期间，遇到了，其实应该是对于抓包软件通用的问题：

* 问题：
  * 背景=前提=背后的逻辑：对于Android和iOS等移动端：对于全局的网络流量，只能有一个控制着 == 一个VPN在用
  * 需求=想要实现：用Reqable去抓包期间，且同时给移动端有想要开启全局代理的话，典型的，比如：`iPhone`中的`Shadowrocket`、`Android`端的`Clash`等代理软件
  * 出现问题：则此时就会互相冲突，开启了其中一个，就会把另外一个顶掉=冲突掉=关闭掉 -> 同一时刻，只能开启一个，要么是Reqable去抓包、要么是`Shadowrocket`/`Clash`等的翻墙代理
* 解决办法
  * 对于Reqable支持：二级代理
    * 概述：把（`Shadowrocket`/`Clash`的）翻墙代理，移动到（协同抓包的）Mac中Reqable的额外配置的（翻墙）代理中
      * -> 即可实现，iPhone中用Reqable抓包，出口流量走Mac的额外的翻墙的代理
        * 实现最初的目标：能同时给iPhone用Reqable的抓包的同时，又能让iPhone中的网络流量实现翻墙（能访问外网）
    * 详见：[二级代理](../features/secondary_proxy/README.md)
