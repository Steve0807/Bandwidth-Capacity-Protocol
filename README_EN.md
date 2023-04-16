# Triode
> <a href="README.md">中文</a> | <a href="README_EN.md">English</a>
>
> In electronics, a Triode can be used to control a larger current with a smaller.
> 
> And the project Triode enables the use of a small network bandwidth to control a very large pool of bandwidth and relay data.

### Triode is a specification, and an implementation that conforms to the Triode specification should be able to perform the following functions:

* Establish UDP tunnels between any two clients.
* At the same time , no traffic needs to be relay by a server.

### Most of the content of this project is on [Wiki](https://github.com/Xor7Studio/Bandwidth-Capacity-Protocol/wiki), Before reading the Wiki, please ensure that you:
* have **_read_** and **_understood_** most of the content on [How NAT traversal works](https://tailscale.com/blog/how-nat-traversal-works/) .
* Capable of establishing connections between Easy NAT to Easy NAT and Easy NAT to Hard NAT in **_non-extreme_** situations.

### The wiki will use most of the definitions in the article, but at the same time make slight adjustments to some of the definitions in the article.
* We also refer to devices on the public network as Easy NAT.
* We will **_only_** refer to **_Symmetric NAT_** (Can be found in [RFC 4787](https://www.rfc-editor.org/rfc/rfc4787), it as a type of Endpoint-Independent Mapping in sections 4.2 and 4.3.)   
as Hard NAT, **_without_** considering other special NAT types for now.
