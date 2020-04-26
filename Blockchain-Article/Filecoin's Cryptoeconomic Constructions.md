# Filecoin's Cryptoeconomic Constructions
# FILECOIN的加密经济学结构

![FilecoinsCryptoeconomicConstruction](https://filecoin.io/images/blog/filecoin-cryptoeconomic-constructions.jpg)

Public blockchains rely on a combination of cryptography and incentive structures that make a system work without centralized control. Cryptography makes some harmful actions practically impossible, while game theory discourages others. Analysis that focuses on this set of mechanisms is called cryptoeconomics. A properly-structured cryptoeconomic system can determine whether a network becomes valuable and self-sustaining or struggles to get off the ground.
公链需要结合密码学技术以及激励机制才能让系统在不受中心控制的情况下正常运作。密码学的存在让一些难以实现的操作得以进行，但博弈论的存在又让人与人之间的合作变得困难。分析并解决这些问题的机制便是*“加密经济学Cryptoeconomic”*。一个结构合理的加密经济学系统可以让一个网络有价值且自洽，反之则会让网络难以维生。

Filecoin’s mission is to create a decentralized, efficient and robust foundation for humanity’s information. To advance that mission, we’ve created a decentralized storage network that lets anyone in the world store or retrieve files. We hope Filecoin will make storage cheaper and more reliable by helping small players compete directly with well-known centralized services, providing a common interface for providers of all sizes, and greatly reducing migration and transaction costs.
Filecoin的使命是创造一个去中心化的，高效的，高容错性的，为全人类信息服务的基础设施。为了达到这个使命，我们构建了一个可以让世界上所有人储存和检索文件的去中心化储存网络。通过扶持中小企业并与知名中心化储存供应商竞争，为供应商提供各种通用接口等手段，我们希望Filecoin会让储存成本更加低廉而可靠，大大降低数据迁移与交易的价格。

Today, we’re pleased to provide an overview of the cryptoeconomic structures that will allow Filecoin to create that foundation. Filecoin uses a combination of existing cryptoeconomic structures and many new ones to meet the network’s unique requirements. If you’re interested in Filecoin’s long-term success as a storage marketplace, you should find these mechanisms encouraging. While we’re still conducting extensive testing to finalize parameters, we’re excited to share these details on how the system works.
今天，我们很荣幸地向大家介绍Filecoin的加密经济学结构，它是Filecoin的基础。Filecoin将已有的加密经济学结构同许多新概念相结合，满足网络中各种独特的需求。如果您长期看好Filecoin在储存市场的发展，您也会被其背后的机制所吸引。尽管目前我们仍在进行大量的测试以敲定最终方案，但我们仍然很高兴能分享Filecoin运作的相关细节。

![Pic1](https://filecoin.io/images/blog/filecoin-cryptoeconomic-chart.svg)

### An overview of Filecoin’s economy
### Filecoin经济模型概览

There are five main actors in the Filecoin economy:
1. Clients, who store and retrieve data via applications.
2. Developers, who develop applications on top of the protocol.
3. Retrieval services, which deliver files to clients on demand.
4. Storage miners, who store files and help maintain and update the Filecoin blockchain.
5. Token holders, who make Filecoin a viable currency by using it as a store of value and as a medium of exchange.
在Filecoin经济模型中，有五类重要角色：
1. 储存客户，通过应用储存或检索数据
2. 开发者，基于协议开发应用
3. 检索提供商，向客户推送其需要的数据
4. 储存矿工，储存数据，维护并更新Filecoin区块链
5. 持币者，通过将FIL用作储值手段和交易媒介，令Filcoin成为一种可用的货币。
