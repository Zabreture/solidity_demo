#### 学习历程：

·我实现的是==网页==前端通过后端==JavaScript的Web3模块==与协议相连，整体的思路框架大概如下：

![image-20220114153219316](https://github.com/Zabreture/solidity_demo/blob/main/src/image-1.png)

#### Solidity的学习

·底层理论学习：

[Solidity中文文档](https://learnblockchain.cn/docs/solidity/)：翻译自官方文档，里面较为详细的包含了Solidity的相关内容，有些较为底层，可以挑重点读。

[Solidity教程](https://www.qikegu.com/docs/4813)：与上面相比较为简化，但可能也有疏漏且最近编辑时间是2019年(Solidity属于新出的语言，版本更迭较快，不同版本之间也有很大差别)，可以先看本教程，同时结合上述文档查缺补漏。

·实际操作学习：

[CryptoZombies](https://cryptozombies.io/zh/)：该教程上手简单，通过编写游戏的方式简单介绍了从协议编写到与网页连接的过程，在实际编写中可以参照本教程(在前后端连接的时候，该教程并未使用框架，所以使用Web3模块是通过下载包含本地文件实现的)，只需要看前6章的内容。

#### HTML与JavaScript的学习

·网上有很多文档这里推荐一个比较系统的[文档](https://developer.mozilla.org/zh-CN/docs/learn/JavaScript)，可以大概略读JavaScript的简单操作，有一个大概的整体框架。

#### Web3.js模块的学习

·[Web3.js中文文档](https://learnblockchain.cn/docs/web3.js/)：与上面的中文文档类似，翻译自官方文档(翻译时存在部分未完全翻译的页面，可以略读或者跳过)。

#### 协议的部署

协议有很多中部署方式，本次采用了Infura以及MetaMask部署

[MetaMask](https://chrome.google.com/webstore/detail/metamask/nkbihfbeogaeaoehlefnkodbefgpgknn?hl=zh-CN)：一个浏览器扩展程序(安装需要翻墙)，相当于一个支付宝或微信钱包，只不过是分布式的。

[Infura](https://infura.io/)：一个在线的以太坊服务器，可以简单的通过它连接接入以太坊。

[Remix](https://remix.ethereum.org/)：在线的以太坊协议编辑器，提供在线的编译器、调试器和协议部署(就是通过它来部署协议)，但是编辑手感可能不太好，下面会介绍我使用的编译方式(当然也可以按照自己的习惯来，顺手就好)。

协议部署大概分为以下几步：

Step1：注册MetaMask并连接到测试链获得测试以太币，在Infura上建立工程得到**工程地址**(CSDN上有现成教程，挺简单的)

Step2：将要部署的文件通过Remix打开：

![image-20220114154114067](https://github.com/Zabreture/solidity_demo/blob/main/src/image-2.png)

点击这个选项后MetaMask拓展会有链接提示，点击部署也会有提示(因为部署需要花费以太币)。

Step3：部署成功后在Remix命令提示行中会有**合约地址**，协议部署完成。

协议部署成功后得到合约地址和工程地址用于web3交互链接(具体方法在上述实践操作教程中有)。

#### IDE

这算是我的一个小习惯，每次学习新语言总想用比较顺手的编辑器。

我采用的是Solidity：Vscode添加插件与在线Remix或MetaMask相连，HTML&JavaScript：WebStorm。

这两个IDE语法提示、高亮等方面都比较方便。(先利其器哈哈哈)

