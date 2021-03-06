---
layout: default
title: '透明计算：不透明的科学大奖'
date: 2015-01-24T00:00:00.000000+08:00
author:
    display_name: 
---

透明计算：不透明的科学大奖

中国新闻周刊记者/钱炜

2015年1月9日，2014年度国家自然科学奖揭晓，一等奖授予了中国工程院院士、清华大学教授张尧学及其所率领的团队，获奖成果是一种全新的“网络计算的模式及基础理论研究”，简称“透明计算”。

作为中国自然科学领域的最高奖，国家自然科学奖一等奖向来以宁缺毋滥而著称，在1999年～2013年的15年间，该奖有过10次空缺。因而，此次透明计算的获奖立即引起各方关注。

首先，由于张尧学是现任中南大学校长，所以他的获奖身份难免引起疑惑。为此，他在微博上回应道：由（应为“根据”——编者注）国家自然科学奖申报规则，2014年只能申报2011年1月1日前取得的科研成果。因此，尽管我申报时填写的是中南大学，但系统根据我的论文发表单位，自动更换成了清华大学。这次获奖仍然是属于清华大学和中南大学两家的，这是清华和中南的共识。而且，自然科学奖规定只奖励个人，不奖励单位。希望各位校友和师生理解。

实际上，针对张尧学获奖的争论远不止他以什么身份获奖。在新浪微博、知乎和清华水木BBS上，很快就出现了“这是科学界的一个笑话”“自然科学奖的一次裸奔”等评论。在国内最主要的科学社区“科学网”上，张尧学获奖的新闻一度有61条评论，这些评论呈现出“一边倒”的质疑声，然而，两天以后，这条新闻的相关留言已全部被删，且被取消了评论功能。

某国家级计算机研究机构的A教授在发给《中国新闻周刊》记者的邮件里说，“这次事件最大的害处是劣币驱逐良币。请不要提我的名字。”

透明计算究竟是一个怎样的学术成果？有没有资格拿国家自然科学一等奖？报奖和评审程序符不符合规范？带着这三方面的问题，记者采访了多位计算机科学界的权威人士。不过，几位受访者均不愿暴露自己的姓名。

透明计算怎么算

综合已有的公开信息，张尧学的“透明计算”的基本思路，是通过网络将存储、计算与管理分离，不仅把数据和应用软件放在云端，而且把“计算机的大脑”——操作系统也放到了云端。在使用时，用户只需通过个人账号登录电脑、手机、PAD等任何终端，就能从指定服务器调用数据和软件，把当前终端变成自己常用的电脑。而终端只下载了用户调用的相关软件和数据，使用后的数据更改和用户习惯仍保存在服务器里。

对一般人而言，这听起来有些像云计算。

记者采访的专家B与上述A教授同属一个研究机构，他的研究方向为高性能计算机体系结构与操作系统，与张尧学的研究领域类似，是学术界俗称的“小同行”。他告诉记者，计算机界一直有一个理想，就是让资源在网络上无处不在，用户只需要一个最简单的终端就可以调用它们。这就像供电系统一样，电器插上即用，而不用管电是从哪里来的。

为了实现这一愿景，1990年代初，网格计算的概念开始兴起。后来，又有了普适计算、效用计算……直到2006年左右，IBM提出了云计算。“网格计算是学术界提出来的，云计算是商业界提的，最后是云计算的概念胜出。国内现在做云计算研究的人，大多都是从当年做网格计算转过来的。而透明计算也与此类似，它们要达到的最终目的都一样，但技术上的实现途径不同。”

中南大学的学生们曾在一首改编歌曲《张校去哪儿》中，将张尧学称作“欧巴”（韩语，意为哥哥）。借用这个典故，上海的计算机从业人员林沛满写了一篇分析透明计算的文章，并且起了一个调侃式的标题——“我为欧巴献计忙”。这篇文章在IT圈广泛流传，作者自己称，在新浪微博上有30万的点击量。

在文中，作者分析说，在实现技术的途径上，透明计算与云计算、远程桌面（VPN）都不同，而更接近于1984年就已出现的PXE Boot（预启动执行环境），即一种使用网络接口启动计算机的机制，可以让计算机的启动不依赖本地数据存储设备（如硬盘）或本地已安装的操作系统。

对于上述解释，专家B表示，PXE Boot通过局域网加载一个操作系统，这一点是和透明计算非常像的。可以说，透明计算扩展了PXE Boot这种模式，增加了更多的灵活性。

然而，透明计算的实现制约于带宽。这位专家解释说，操作系统的映像是非常大的，即使是只加载启动必须的程序，也同样对网络带宽有较高要求。这是因为，越贴近应用层，越了解真实需要的数据，所需要下载的数据就越少；而越往操作系统底层，甚至到了块设备的层次，不了解准确需求，需要下载的数据就越多。现在的带宽平均只有20Mb/s，而透明计算要求的带宽是它的100倍。因此，透明计算虽然可能具有更好的通用性，但性能不会好。“其实，当年网格计算没实现，关键也是带宽没跟上。”

被包装的“透明”？

在张尧学因透明计算而获奖后，《光明日报》《中国科学报》等媒体皆以“颠覆了计算机的冯·诺依曼结构”为亮点报道了这一成果，这句话也成为大家激辩的最大的焦点。对此，专家B表示，只要仍是半导体制成的电子计算机，就不可能摆脱冯·诺依曼结构。只有目前还在研究的生物仿生计算机与量子计算机，才有可能跳出这一结构的藩篱。

记者注意到，实际上，张尧学的公示报奖材料中并没有使用“颠覆”一词，而只是用了“扩展冯·诺依曼结构”这样的叙述。

被众人“围剿”的另外一点，是英特尔公司的一篇演讲。根据2012年清华大学的一篇新闻稿，在该年9月在旧金山举行的英特尔美国信息技术峰会（IDF）上，英特尔高级副总裁、软件和服务集团总经理詹睿妮做了题为“透明计算时代的安全和服务”的主题报告。这篇新闻稿写道：“在报告中，詹睿妮高度评价了由我系张尧学院士提出的透明计算。詹睿妮指出，‘透明计算是由张尧学教授所倡导的，使应用程序跨越操作系统和体系结构无缝运行，是把用户放在计算体验的中心的一种新计算模式’。”

詹睿妮的这段演讲被作为透明计算获得“同行评议”的一条重要依据，被张尧学展示在自己清华大学官网的个人简介上。记者仔细观看了这段长达50多分钟的演讲视频，发现詹睿妮只在第14分钟左右提到了清华大学和张尧学：“透明计算这一概念并不新鲜，它最早从1990年代晚期开始，实际上在麻省理工学院就有人做这方面的工作。最近是在位于北京的清华大学，由一位张教授在做，我说不出他的名字，我们一直以来在和他进行合作。”

在英特尔公司发布的“2011清华—英特尔透明计算与云计算技术研讨会”的新闻稿中，还有这样一句话：“透明计算技术是云计算在中国应用的一个很好的案例。”

实际上，根据A教授的检索，有关透明计算的文献分别在1989年、1999年与2001年都能找到。其中，正式提出透明计算概念的是美国施乐公司的首席工程师马克·威瑟，时间是在1980年代晚期。而张尧学则是在2004年提出这一理念的。

根据《国家科学技术奖励条例》规定，自然科学奖必须具备三个条件：前人尚未发现或尚未阐明；具有重大科学价值；得到国内外自然科学界的公认。从以上事实来看，张尧学并非是第一个提出透明计算概念的人。此外，尚未发现有迹象表明，他的这一成果已经受到国际学术界的认可。

2012年10月出版的《国际云计算杂志》以长达百余页的专辑形式介绍了张尧学的理论。这本英文期刊的主编为美国乔治亚州立大学的潘毅教授。张尧学的公示材料里也有一句话：“相关论著被美国教授 Y. Pan （潘毅的英文名字——编者注）评论为‘可能是该领域的里程碑’。”

而实际上，潘毅是张的朋友，同时也是中南大学的客座教授。在张尧学的个人简历上，还附有一篇由潘毅所写的文章——《集科学家、作家、高管于一身——记我的好友张尧学院士》。在这篇发表于2009年的文章的一开头，潘毅写道：“在当今中国社会里，从作家成为一名高官不算新鲜；既是科学家又是高级干部也非屈指可数。但集高官、科学家及作家于一身的人，恐怕是凤毛麟角的了。当今的教育部高教司司长张尧学院士就是这样的一位突出的奇才。”根据该文所述，张尧学与潘毅是从1998年开始在日本认识的。文中所提到的行政职务是张尧学在2011年调任中南大学以前所担任的。

根据A教授的检索，第一获奖人张尧学的论文最高引用次数是46，“你可以对比一下自然科学二等奖或美国一个助理教授的论文引用量”。对于这一点，记者采访的另一位不愿透露姓名的教授C也表示，“申报材料里列出的论文，只有个别属于高水平，但总体看起来还比不上我们单位里申报教授的材料。”

不过，有人觉得透明计算的获奖也算正常。北京一所同时属于“211”与“985”工程的重点大学计算系张教授表示，这几年云计算比较火，透明计算的概念与此接近又有所创新，这是它能获奖的重要背景。“赶上了好时候，而且他很会用词，透明计算这个概念很抓眼球，能给人留下深刻印象。咱们搞学术的，起个好名字很重要。”

C教授则在微信中向记者表示：“此前一些媒体的质疑也有些过头。不能说透明计算完全没有价值，这毕竟也是一次学术探索，不属于造假行为，顶多说是为了创新而创新。计算机属于工科，是应用科学。透明计算得个技术发明三等奖或二等奖或许都没问题，但竟然拿走了自然科学一等奖，这有些过了。”

不够透明的评奖

实际上，早在2004年，张尧学就用同一成果获得过国家技术发明二等奖。只不过，他当年的获奖成果叫“索普卡电脑”。媒体报道对索普卡电脑的描述是这样的：“它本身是台裸机，没有任何软件，计算机运行所需的操作系统软件和应用软件都能从服务器下载得到。而且这种下载是根据用户要求，只下载当前在计算机上运行的一小部分指令，不是操作系统和应用程序全部。如此，传统计算机所必需的大存储器可以减小，CPU也减小，许多附加部件不要了。”该电脑为2001年研制成功，张尧学为第一完成人。

记者把相关报道发给在某权威性计算机研究机构工作的D教授，向他求证索普卡电脑是否就是透明计算概念的实体，此说得到了他的肯定。同时，他也表示，在已经获得了技术发明奖之后又用相同的理论去申请另外一个奖项，不符合国家不允许重复报奖的规定。

实际上，张尧学在1999年就离开了清华，先后就职于教育部、国务院学位委员会，直到2011年年底才回到高校，担任中南大学校长。由此可推断，他在研发出了索普卡电脑之后，长期担任行政工作。这也是引发众人怀疑的背景因素：一个长期实际担任行政管理工作的官员，怎么有精力去做科研并取得如此重大的成果？

为了具体了解国家自然科学奖的评审过程，《中国新闻周刊》记者试图找到参与此次评奖的专家，并为此联系了国内计算机领域的4名院士。其中，联想集团首任总工程师、76岁的倪光南和中科院计算所所长李国杰的研究领域与张尧学接近，但他俩皆向记者确认：并未参与此次评审。网络安全专家、原北京邮电大学校长方滨兴在电话里表示目前身在在国外，暂不便答复。而图灵奖（国际计算机领域最高奖）得主、清华大学教授姚期智对此未有回复。

国家科技奖励办公室宣传处一位李姓处长在电话里表示，这次评奖从2014年1月份就开始，到10月结束，历时10个月，是很慎重的。奖励办只是评奖的组织单位，对评选结果没有发言权，评审专家的名单也是保密的，不能公布。

但倪光南的说法却与此相反，他在短信中建议记者去找评审专家问清楚情况，并强调，这份名单并不是保密的。同时，他也表示，“猜有关部门可能想淡化处理此事”。

就上述种种疑问，记者致电张尧学的秘书林老师要求采访，但被婉言谢绝。腾讯科技称，他们在联系张尧学本人采访未果后，又试图联系清华大学计算机系一位陈姓教授，该教授曾参与过透明计算的研究工作，希望他可以从专业角度解答公众质疑，但这位教授表示，现在事情正处于舆论焦点，不方便发表评论，“科技的东西，因为公众很难理解，怎么说都会有问题”。

不愿透露身份的业内专家D教授在给《中国新闻周刊》记者的邮件里最后写到：呼吁国家“透明”评选过程！

(XYS20150124)

