# Triode
<p align="right">
  <a href="README.md">中文</a> |
  <a href="README_EN.md">English</a>
</p>


> 在电路中，三极管可以使用较小的电流控制较大的电流，
> 
> 而Triode项目则可以使用较小的带宽去控制非常大的带宽池，并用于中继数据。

Triode是一个规范，符合Triode规范的实现应能实现如下功能：

* 在任意两个客户端间建立UDP隧道
* 实现第一项的同时，无需服务器中转任何流量

### 本项目的大部分内容都在[Wiki](https://github.com/Xor7Studio/Triode/wiki)中，但在阅读Wiki前，请确保您：
* 已经阅读并理解了 [NAT 穿透是如何工作的](https://arthurchiao.art/blog/how-nat-traversal-works-zh/) 中的大部分内容
* 能够在非极端情况下穿透Easy NAT-Easy NAT，Easy NAT-Hard NAT，并建立连接

### Wiki将使用文章中的大部分定义，但同时对文章中的部分定义做出了微调：
* 将公网环境也称之为Easy NAT
* 仅将Symmetric NAT称为Hard NAT，不考虑其他特殊NAT类型情况。
