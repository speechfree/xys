---
layout: default
title: '泼点冷水，海思的备胎芯片能救华为吗？'
date: 2019-05-21T00:00:00.000000+08:00
author:
    display_name: 李斌
---

泼点冷水，海思的备胎芯片能救华为吗？

作者：李斌　　来源：书斋闲话

最近中文媒体圈里何庭波给海思员工关于启动所谓备胎芯片的信刷屏了。我读了之后，却觉得有些话不得不讲。

对于业内人士来说，这封信就是在忽悠外行，给吃瓜群众打鸡血的。设计芯片和设计线路板使用芯片，是两回事。她的团队已经开发了三五成的替代芯片，或是只是设计出了核心功能芯片。她可能以为虽然功能差一些，觉得也能凑合着用。但是一个产品上的线路板，少一个芯片就没办法生产。而一个产品少则几十，多则成百上千个芯片，其中大多都是通用芯片，是欧美公司几十年的累积经验研发出来的。

我是相信中国人的聪明才智的，华为更是聚集了国内菁英。如果华为集中人力，花几年的时间，开发出一个管脚和功能相同的通用芯片，这已经是很了不起的成就了。现在国内自己研发的芯片，几乎都是专用芯片ASIC （Application-Specific Integrated Circuit），也就是根据自己产品的需求，量身定制的。这种芯片不愁销路，没有竞争对手，随着自家产品而进入市场，而其芯片本身并没有商品的竞争对手、价格、供需等特性。

笔者在设计硬件线路领域已经有二十多年了，在这方面比搞芯片设计的人更有发言权。我前后工作过的几间大公司对于产品选用芯片的流程几乎相同。

首先设计所用的元器件（包括芯片、电阻、电容器、晶振、二极管等等）都需要从AVL（Approval Vendor List）的厂家中选取，除了保障产品质量，还有一点就是保障供应的可靠连续性。除此之外，这些元器件大多需要second source, 就是管脚功能一模一样的第二、第三个厂家。只有极个别的可以例外，如Intel的CPU、PCH，Broadcom、Marvell 的通信芯片系列等。除了它们的芯片提供主要功能，独一无二的之外，还有就是它们都是芯片大厂，可靠性有保障。

对于其它辅助功能的芯片，虽然有两三个厂家，但我们也常碰到芯片EOL（end of life)的通知。这时候通常根据自己产品预计生产的年限和所需量做一次性的LTB (last time buy)。当然如果买的芯片不够，或预计自己的产品的生命周期在几年内都不会结束，那么这时则需要找功能类似的芯片，修改原理图和线路板，同时也要修改BOM（build of material) 。等新的线路板生产回来后，还需各种测试（dvt，dmt，emi?）以及后续的report，快则两三个月，慢则半年。这还只是少一个芯片，并能找到类似功能的情况。如果找不到类似功能的芯片，那么这个产品就可以洗洗睡了。

在全球化、产业分工越来越精细的今天，对于华为这样一个使用大量通用芯片的公司，断芯就意味着断粮断水。海思是绝无丝毫可能设计出满足华为产品的全部芯片，甚至于连一半所需芯片也设计不出来。如果何庭波误以为海思把华为所需的关键核心芯片的备胎设计出来，就可以救华为，那就是太无知了。少了不起眼的辅助芯片，如供电芯片、桥芯片、数模转换芯片等等，就像少了空气一样，虽然平常不觉得它存在，但一旦缺失，就会窒息而死。

对了，还忘了说芯片设计辅助软件，美国在这方面几乎垄断了。

所以，只要美国断芯（美国芯片生产占世界芯片总量一半以上），华为是九成九死定的。那百分之一生存的可能，就是中国闭关锁国，关起门来发展，不再参与全球竞争。而这样做的代价，恐怕是中国乃至全球都难以承受的。

考虑到何庭波并不是个外行，更可能的一种情况是，她这封信有一个前提——中美贸易战还有缓和的余地。一旦缓和，美国解除或放松对华为的禁令，华为通过将海思的备胎芯片转正，逐步提高芯片的自给率，增强华为在中美贸易争端背景下的生存能力。这个做法当然是可取的，但以此忽悠民众在中美贸易争端中盲目自信就不对了。

编者注：本文作者之一李斌为上世纪末移居美国的中国大陆留学生，目前在美国从事电子硬件行业设计已经有20年，使用过各种类型的芯片，日常跟各种半导体厂商打交道。

(XYS20190521)
