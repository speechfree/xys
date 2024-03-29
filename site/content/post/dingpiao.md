---
layout: default
title: '优化订票流程，解决铁路网上订票系统的困境'
date: 2012-01-12T00:00:00.000000+08:00
author:
    display_name: 野有蔓草
---

优化订票流程，解决铁路网上订票系统的困境

作者：野有蔓草

铁路网上售票系统12306网站由铁道部信息中心和中国铁道科学研究院共同开发，铁道科学研究院电子所负责开发和维护，于2011年6月1日正式上线。春运开始以来，12306.CN备受责难，旅客通过网络售票网站购票时，频频遇到网络“堵车”现象，新用户无法注册，订票遭遇“系统忙”干扰。

铁路部门将原因归结为网站访问量过大，导致技术无法承载，造成了系统出现故障，将采取诸如增加带宽、加快技术维护等一系列措施。最新消息是，铁道部门针对全国“一张网”网络瘫痪状况，正研究实施“开分店”式多网运作减压，因时间问题不可能今年春运实现。明年春运或试行。

网上IT强人、其他电商架构师则分析了12306前端、数据库、软件问题，认为当前系统设计实现有问题，没有进行充分的压力测试，也很有道理。

也有洗地的：如清华Web与软件中心电子商务研究室主任王津：“中国的铁路电商系统，将是全世界规模最大的电商系统之一，也是全世界最海量最高速的事务处理系统之一，运行峰值时没有任何已知的系统可以比肩，是难度最高最容易失败的系统之一。”

媒体评论员则一贯正确的归因为网络购票被垄断、售票网站建设招标不公正、体制问题等等。

理论上讲，12306系统就是一个的排队系统，窗口忙即时拒绝，客户为了抢票立刻再发起请求，又加剧了系统负荷，形成雪崩效应。日均点击次数超过了10亿次，平均每天有不到200万旅客成功通过网络购票，平均刷屏超过500次才能买一票，可见这个排队系统服务质量太低了。如果换成电话系统，平均试呼500次才能接通一次，大家是否觉得这样的系统可以接受？

那么，问题在哪里？这跟当前网络售票的流程有密切关系，售票时间为每日6点至次日凌晨1点，当然是越早订抢到票的可能性越大，所以6点整全国几百万的人同时开始拼命刷新12306页面，这就形成了巨大的并发点击峰值，当然系统可同时处理事务数是有限的，大多数用户只有遭遇“系统忙”，一再刷新。

网站硬件系统升级、带宽扩容、软件优化、甚至采用“开分店”式多网运作等方法当然能改进服务质量，但也无法避免点击峰值产生及系统忙。更值得注意的是，很快就会有各类刷屏或秒杀工具出现，刷屏将成数量级增长。

峰值最高超过14亿次点击的确是全球最繁忙电商系统，但每天200万张订单在电商中却不算大。参考：淘宝每日订单数达800万, 淘宝商城“双11” 活动订单数超1000万。京东商城每日30万订单量。导致12306高并发点击困境的是因为不合理的订票流程：只有抢在最前面下单才有机会订到票。

根本问题不是投入更多的设备及网络资源建设一个能处理峰值超过10亿次点击的全球最大电商系统，而应以方便乘客购票、高效低成本地支持日发售200万张车票为目标。将春运时期订票系统拆分成预订、抽签、交易三个部分可有效解决：

【预订票子系统】：用户查看剩票信息，输入席次、乘车人信息等全部必要信息，提交订单。

【抽签子系统】：预订阶段结束后，系统导入全部订票申请进行处理，按席次分类排队，随机抽签，抽中的申请即预分配车票。系统随后通过邮件及短信给用户发送是否抽中的通知。

【交易子系统】：用户收到抽中短信通知，只需要指定的时间内登录网站完成交易即可。

这样改动后，用户只需两次成功登录即可完成购票过程，成功率与登录时间先后无关，这样旅客无需挤在第一时间抢票，点击负荷很自然分散到整个服务时段，避免点击峰值产生。各阶段时长可按统计及模拟结果分配。削去购票峰值后，整个系统对硬件、带宽的要求就大为降低，更关键的是降低了全民在购票时的时间成本。只要总运力与乘员数相匹配，乘客迟早可买到票。为公平起见，抽中而未取票者，后续抽签优先级降低。

春运电话订票一直以来也是非常难以打通的，其实也可以融合到以上流程，电话订票申请单导入后台后统一抽签，结果短信通知乘客到实体窗口取票。这样也给农民工等不方便上网部分用户公平购票机会。实名制手机通过短信预订车票方式也值纳入得考虑，短信是存储转发机制实现的，几乎没有负荷瓶颈。

(XYS20120112)

