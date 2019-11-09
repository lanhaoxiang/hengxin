# 恒信可信网络白皮书

## 简介

恒信可信网络是基于 TEE（可信执行环境）和 DAG（有向无环图）技术构建的开源的、不可篡改的网络数据库。它的优势主要体现在以下三个方面：高性能，低成本，可不依赖奖励机制。

## 1. 概览

区块链技术巧妙地使用 [PoW 共识机制](https://en.wikipedia.org/wiki/Proof_of_work)解决了分布式网络中一度被认为无法解决的拜占庭将军问题（[Byzantine Generals Problem](https://en.wikipedia.org/wiki/Byzantine_fault)，*q.v.*: [LESLIE LAMPORT，1982](https://people.eecs.berkeley.edu/~luca/cs174/byzantine.pdf)），创建了世界上第一个不可篡改的分布式账簿（即，比特币的账簿）。同时，因为这个账簿是由分布式网络中的众多节点共同维护的，所以，伴随着不可篡改，也自动拥有了一些其它属性，比如公开、透明。

自比特币这个世界上第一个被证明为可行的区块链应用横空出世以来，在随后的十年左右的时间里，人们一直在探索将这样一个不可篡改的分布式账簿应用到众多领域之中 —— 毕竟，一个公开、透明的，不可篡改的数据库，应该是很多场景的刚需。

PoW 的不便之处需要耗费大量的算力（成本相对较高），而 [PoS](https://en.wikipedia.org/wiki/Proof_of_stake)（以及它的改进版，dPoS）虽然网络维护成本相对于 PoW 低很多，可依然无法彻底突破真正可落地的实际应用所需要的高并发性能。

而恒信所采用的基于 TEE 与 DAG 结合的方案，使用异步的、容忍拜占庭过错的共识机制，创建了一个高性能、低成本且可以不依赖奖励机制的健壮分布式网络数据库。

### 2. 系统稳定性

恒信网络，是 [Mixin Network](https://mixin.one) 的非商业开源版本。

Mixin Network 自 2019 年 2 月正式上线以来一直处于无差错稳定运行状态；Mixin Network 中总计管理 1,144 种数字资产（这个数字还在不断增加），累计处理过亿交易记录，峰值 TPS（Transition Per Second）为 198（2019 年 11 月 9 日）—— 事实上，**Mixin Network 不受任何 TPS 限制**。https://mixin.one/snapshots

