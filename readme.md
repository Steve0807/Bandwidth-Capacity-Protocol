# Bandwidth Capacity Protocol

## 前言

欢迎来到带宽电容协议（BCP）的文档！

本文档默认您：
* 已经阅读并理解了 [NAT 穿透是如何工作的](https://arthurchiao.art/blog/how-nat-traversal-works-zh/) 中的大部分内容
* 能够在非极端情况下穿透Easy NAT-Easy NAT，Easy NAT-Hard NAT，并建立连接

本文档将使用文章中的大部分定义，但同时对文章中的部分定义做出了微调：
* 将公网环境也称之为Easy NAT
* 仅将Symmetric NAT称为Hard NAT，不考虑其他特殊NAT类型情况。

## 基本原理

好了，现在你知道Easy NAT-Easy NAT与Easy NAT-Hard NAT情况是可以直接打洞穿透的，而Hard NAT-Hard NAT无法直接穿透，需要使用中继，对吗？

一般情况下，很容易想到使用中心服务器中转，对吧？但对于用户众多或带宽占用较大的应用（很不幸，Minecraft:Java Edition这俩项都占了），这种思路会导致中转服务器（或服务器群）压力巨大，进而带来大量的运营费用。

到这里，你肯定会问：那BCP是如何解决该问题的呢？

其实很简单，BCP用到了很久前的技术：分布式P2P。只不过之前这种技术被用于P2P下载，而我对其进行了一定更改，以用它中继数据。

BCP将要求Easy NAT用户共享出自己的一部分空闲带宽，并用网络中的所有这些空闲带宽中继Hard NAT-Hard NAT情况下的流量，因为Easy NAT用户众多，所以带宽在大多数情况下足够使用。

BCP将使用端到端加密以保证数据安全。

## 更多内容

请参阅[Wiki](https://github.com/MC-XiaoHei/Bandwidth-Capacity-Protocol/wiki)