---
title: 实验室使用和维护指南
date: 2018-12-12 14:40:44
categories: Maintenance
tags: 实验室维护
---

</br>
<center>2017 何剑锋 2016张渝宁 </center>


## 概述
![301工作室](/asset/images/301-fig.jpg)

301工作室是CUPT比赛期间的工作场所，提供相比实验室更加优雅整洁的环境。

除了查资料、看文献、写代码、处理数据、画图、跑计算模型之外，你还可以在301吃外卖，喝咖啡，通宵，睡觉，甚至开party。。。（误）
同时下一届纳新之前301同样作为工作室，进行面试和各种培训指导。

当然，301同时也提计算服务器资源，无线网路，并且作为图书馆存档历年的文献和荣誉。通常来讲，比赛期间团队所有文献和理论工作都在301进行，保持整洁是301的首要要求。

![302实验室](/asset/images/302-fig.jpg)

302位于301的对面，主要用途是做实验及存放实验器材。日常需要用到该实验室的项目主要是CUPT，但在卓越杯举办期间也会用做卓越杯的实验场地。

值得注意的是，仅有302的左侧是竞赛可使用的实验场地，右侧是一位老师的工作场地，在使用时切勿走错，以免造成麻烦。

实验过后请及时进行清理打扫，否则实验室很快会变成一团乱麻。

### 功能分区

#### 301 工作区
##### 办公桌
进行桌面工作，查资料、看文献、写代码、处理数据、画图、跑计算模型，吃外卖等等。日常工作期间随来随用，可以放置个人物品，甚至主机电脑，空间足够基本不会出现没有位置的情况。

暑假集训期间由于所有队员都长期驻扎实验室，此时需要固定工作区域。
- 正式队员：固定每人一张，且负责本桌面周围区域的清洁卫生
- 观摩队员：空余一张，负责此桌面清洁卫生

使用时间直到下一届纳新结束前，之后在下一届队员入驻前清理个人物品，完成交接

##### 工作站
301的桌面电脑，自带各类大型软件

1. 承担计算和数据密集任务
2. 部署路由器网桥，使用python脚本实现WiFi广播，登陆校园网可以使用。（见下部分网络服务）
3. 外接打印机/扫描仪可以进行基本的文档打印。
4. 每次比赛完成后对比赛进行归档，包括但不限于过往照片，汇报PPT，代码和数据等等。

##### 网络服务
WiFi是现代人的基本需求，然而重大校园网使用drcom客户端会检测路由广播，发现路由器会将登陆账户踢下线。

解决方案很简单-[drcom上网脚本](https://github.com/drcoms/drcom-generic)

1. 华为网桥接线至路由器蓝色主要端口，路由器附属线链接主机。
2. 卸载drcom客户端换用python脚本进行登陆。
3. 下载drcom库至本地，编辑latest-wired-python3.py脚本，将主机ip设为重大ip(server: 10.254.7.4)，并输入自己用户名密码（username: password:）。
4. Python3以上环境运行latest-wired-python3脚本，进程后台挂机（如有长期账户可以设为后台启动项）。
5. 享受校园网WiFi。

#### 301 休息区
茶桌和沙发，工作之余休闲娱乐放松吹水，打牌开黑，也可以开party大家一起吃大餐，当然沙发也是睡觉的好地方（误）。
认真来说，**不建议在工作区吃外卖**，因为白色桌子很不好清理，大家一起在这里吃外卖才是正途（误）。
![不建议在工作区吃外卖](/asset/images/party.jpg)

#### 存储区
大量储物柜，301储物柜用于文档和书籍以及个人物品，302储物柜用于放置实验器材。 

##### 301储物柜
1. 基本办公用品，计算器，胶棒，A4纸，订书机，便利贴，曲别针，垃圾袋。。。etc
2. 各类书籍，文档，打印paper。
3. 档案，照片，实验室
   
#### 302储物柜

实验室的柜子用以存放各类实验材料及设备，柜子上贴有**标签**以标示分类。实验室存放的实验器材主要分为以下几类：

1. **废弃的实验器材：** 含损坏的3D打印机、吸尘器等

2. **历届竞赛遗留的装置：** 都是一些为满足特殊实验需求而设计的装置，在一般的实验中不大可能会用上。

3. **各类耗材：** 包括有刀片、钻头、3D打印机的原料、胶水、热熔胶胶棒、电工胶带、各类绳及丝、蜡烛（在以往的一次实验中剩下的）、电池、焊锡等

4. **五金相关材料：** 主要是各类螺丝、轴承等。但除此之外还有一些特殊的材料可以用以搭建仪器。
5. **电子相关材料：** 有各类导线、电子元件等
6. **各类工具：** 大致分为五金工具与手持测量工具。五金工具大致包括：常用五金套件、电钻、电磨、电动螺丝刀、电烙铁、热熔胶等。手持测量工具主要包括游标卡尺、千分尺、数字万用表、红外温度计等。
7. **力、热、光、电等方面的实验仪器（大部分是教学仪器）：** 光学仪器主要包括激光发射器及透镜、光具台；力学仪器包括单摆及各类教学仪器；热学仪器主要是几台加热设备及一些热学教学仪器；电磁学仪器主要是电源、各类常见基本电路元件以及磁铁——需要注意，实验室的磁铁大多为强磁，拿取是应当注意，避免手被夹住；且为了保证磁性，不应将磁铁杂乱放置
8. **其它仪器：** 较为典型的有烧杯、量筒、移液器等，除此之外还存有几台近代物理实验的教学仪器。
9. **特殊原材料：** 这一部分比较特殊，一些比较奇怪的实验材料都存放在这里。比如：金属布，甘油，乙醇，各类尺寸的玻璃珠，绿豆、小米、沙子等颗粒物，各种口径的塑料软管。由于材料较多，这里便不一一列举了。

除了以上列举到的设备外，实验室还有一台3D打印机。由于较为常用，其被单独放在一张实验桌上。

#### 302 试验区

专业配电试验台，平时需要做实验时，搭建实验装置材料，当然空间不够的时候直接在地上搭建实验装置也是没问题的。

分配原则同上，平常即来即用，集训时每人分配一张实验桌，并负责相应卫生和维护。

##### 实验注意事项
实验室的维护较为简单，仅需遵循以下原则即可:
1. 每次实验结束后应将桌面材料放置整齐，工具及仪器需放回柜子；实验过程中产生的垃圾亦应及时处理。
2. 最后离开实验室的人员需确保仪器断电（3D打印机不在此列）。
3. 正确使用实验工具，以免造成工具的非正常损坏（如：不得用美工刀调制AB胶）。
4. 使用电钻、电烙铁等易造成人员伤害的设备时应注意安全。
5. 危险品（高温，强激光，腐蚀性毒性化学品）购买使用需要老师了解，实验完毕后妥善储存

除此之外，不得不提一下3D打印机：由于日常实验里大量使用3D打印机，其负荷过大，故障时有发生。遇到该问题时应及时进行维修，同时可以将打印任务委托给物理学院的其他实验室，以保障实验进度。

### 清洁卫生：

1. 工作区实验区按上述分配，由相应队员负责卫生，每次使用完毕后随手打扫
2. 其他区域每周汇报后正式队员一起打扫
- 桌面整理清洁
- 扫地，拖地
- 倒垃圾



