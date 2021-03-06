# 区块链之路

一个零基础、中文友好的上路文集

## 比特币

[一个自己实现区块链的教程，其中也有部分以太坊、卡尔达诺的资料翻译](https://github.com/liuchengxu/blockchain-tutorial)

## 以太坊

- [官方文档](http://ethdocs.org/en/latest/introduction/what-is-ethereum.html)
- [官方文档中文版](http://ethdoc.cn/introduction/what-is-ethereum.html)
- [设计初衷](https://github.com/bsdfzzzy/The-Road-To-BlockChain/blob/master/ethereum/%E8%AE%BE%E8%AE%A1%E5%88%9D%E8%A1%B7.md)

## 卡尔达诺

## 门罗币

## 区块链钱包

### 分类

- 是否联网
  - 冷钱包
  - 热钱包
- 数据存储完整性
  - 轻节点钱包
  - 全节点钱包
- 私钥存储方式
  - 中心化钱包
  - 去中心化钱包
- 主链关系
  - 主链钱包
  - 多链钱包
- 私钥签名方式
  - 单签名钱包
  - 多签名钱包

### 技术实现

1. 钱包自身设计，如何生成助记词，keystore 和密码等
2. 私钥、公钥和地址的产生方法
3. 钱包提供商远程调用各公链 RPC 接口设计

### 钱包安全策略

#### 用户习惯安全引导

- 私钥不随意流转
- 良好的上网习惯
- 重视钱包安全核心要素手动备份
  - 助记词
  - 私钥
  - 密码 + keystore

#### 钱包安全设计

- 网络传输安全体系
  - MITM 中间人攻击防御，即双向校验
  - RPC 调用接口权限安全
- 用户端文件管理安全
  - 安装包文件安全性
  - 抵御终端不良程序对关键文件的访问
  - 终端关键文件加密方式
  - 终端关键文件备份过程显示方式
  - 助记词生成和管理
  - 私钥生成和管理
  - keystore 生成和管理
  - 导入其他钱包生成的私钥和助记词安全
- 开发扩展安全
  - 扩展功能权限管理
  - 用户密码忘记找回功能

## 分布式系统理论

    FLP 不可能性定理：在网络可靠，存在节点失败的最小化异步模型系统中，不存在一个可以解决一致性问题的确定性算法。
    CAP 不可能三角：一致性、可用性和分区容忍性三者无法同时满足，需要弱化某个特性来设计分布式系统。

## 拜占庭将军问题的经典解法

- 口头消息（OM(m)）协议
- 加密消息（SM(m)）协议
