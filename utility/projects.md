# DeFiDefender

基于物联网的动态定价与区块链茶叶溯源系统

## 项目简介

本项目运用了茶叶溯源信息查询系统进行溯源数据的实时监测 ，用LoRa负责数据采集节点与关之间的通信，ESP32对采集数据进行传输，茶叶溯源系统中针对溯源环节的各个场景的数据特点，编写对应的智能合约，进行场景中相关数据的处理操作，不同场景下的IOT设备或者参与人员调用对应的智能合约的接口实现当前场景下的信息数据的链上操作。我们还采用了动态定价根据需求（或其他因素）调整产品或服务的定价，从而使茶农引入多个价格点以增加收益。

## 项目背景

在中国，茶作为我国的传统饮品，光是市面上常见的茶叶就已达百余种，目前我国茶叶消费量已突破两百万吨，光是市面上常见的茶叶就已达百余种，市场规模庞大，且茶叶普遍的价格都较为昂贵。
但是茶叶市场存在散、乱、杂和不易监管等特点，而且在流通过程中，茶叶的好坏没有统一的标准。没有可靠的产品质量保证，新生品牌很难迎合大众，使得有真正卖好茶叶的却销售困难。并且部分不良商家利用信息差欺骗消费者及中间商，以次充好。
本系统利用fisco bcos  多方参与共识， 数据不可篡改的特性，使溯源流程中各环节人员互不干扰，不受限于某一中心机构，让传感器在不同的场景下，对茶叶相关数据进行采集并直接上传区块链，极大程度的降低人为参与的因素，以保证所追溯的信息的真实可信。且利用智能合约自动执行的特点，使得加工商和经销商可以根据市场需求和自身供应能力，以不同的价格将同一产品适时的销售给不同的消费者，或不同的细分市场，实现动态定价以完成企业利益的最大化。

## 项目目标

### 数据有迹可循，茶叶有源可溯：

建立茶叶溯源管理系统，通过给每份茶叶配置溯源码，让茶叶有“身份证”，茶叶溯源管理系统不仅可以有效的监控全国各地茶叶的质量监测，有效打击劣质茶叶泛滥乱象，还能对茶叶设置全国统一的价格防止不同地区乱价现象，真正做到强化茶叶市场价格管理，使市场日趋规范化，不光产品有了保证，企业形象也能因此提高。

### 实行“一茶一码”，市场管理信息化：

茶叶溯源管理系统，实行“一茶一码”，将茶叶从种植到加工，到最后销售的每一环节变得公开透明化，消费者可以通过查询溯源码对茶叶“追根溯源”，获得更多生产信息，销售信息，若出现问题，也可以查清出现问题的环节，“一茶一码”给茶叶贴上“身份证”，实现茶叶市场管理的信息化。

## 方案

物联网传感器采集茶叶种植、加工以及销售各环节信息，同时将信息直接上链储存，利用可信信息进行数据溯源，完成动态定价。

## 应用场景

场景1> 本项目在保证数据的真实可信情况下，采用了物联网与区块链技术相结合的方法。例如，可以应用于第三方的质检。部分商家非法利用市场的漏洞恶意篡改数据，从而导致质检这一过程被操纵，变得毫无意义，但是使用我们系统，在利用物联网传感器采集到的数据上链后进行质检，数据是不可篡改的，保证了质检这一环节的真实公开透明性。

场景2> 应用于消费者的消费过程。随着信息化时代的发展，网购越来越热门，但是，一些不法分子，利用网购买家无法透过网络去实际触摸感受商品，而页面放做工优质商品，发劣质粗糙商品。但是我们系统实行的是“一货一码”制，可以有效的对买家收到的商品进行追溯，必要时可进行追责，使消费者的权益得到了更大的保护。