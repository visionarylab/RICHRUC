RICHRUC
=============

简介
------------- 
这是本人于本科二年级下学期"JAVA程序设计"课程上完成的课程作业——游戏"RICHRUC"。该游戏界面模仿了"寰宇之星"游戏发行商开发的《大富翁7》游戏，完成了大富翁游戏的大部分操作及特性，并结合人民大学的特色，形成了人民大学（RUC）特色版的大富翁(monopoly)游戏。

本项目使用Eclipse开发，因此上传代码为Eclipse项目，可以在Eclipse中直接打开并运行。

注：代码中有一些资源路径放在了绝对路径下(d盘根目录)，若图片或音效资源无法加载则把相应资源放到代码中对应路径下即可。

目标
-------------

Java是目前使用最为广泛的网络编程语言之一。它具有简单，面向对象，稳定，与平台无关，解释型，多线程，动态等特点。它以其友好的开发界面、强大的组件支持等优点，得到广大程序员的接受和认可。

大富翁，是一种多人策略版图游戏。参赛者分得游戏金钱，凭运气（掷骰子）及交易策略，买地、建楼以赚取租金。游戏最终只得一名胜利者，其余均破产收场。大富翁以其功能的多样性，趣味性，画面的精美性吸引了一大批玩家。

本次大作业我们旨在基于JAVA技术实现具有人大特色的大富翁游戏——RUCRICH。其中人大特色指系统机制具有人大特色，功能实现具有人大特色，地图设置具有人大特色三个部分。同时实现大富翁游戏的各项基本功能，保证功能的趣味性、多样性并且设计精美的画面，友好的用户交互界面。此外，在实验的过程中复习、巩固JAVA语言的基础知识，进一步加深对JAVA语言的理解和掌握；掌握JAVA程序设计的思想、流程，及在大项目中的应用；加强理论知识和实际应用的姐和应用，锻炼我们解决实际问题的能力，提高我们的设计能力。



主要目标
-------------
1.载入界面与初始界面

实现了精美的载入界面：当启动游戏后，首先会动态显示中国人民大学的精美图片作为载入动画，给玩家以视觉上的享受。
实现了友好和有特色的初始界面：当载入完成后，进入游戏初始界面，初始界面会提供游戏
操作说明，开发团队，开始游戏，退出游戏等信息，显示方式具有人大特色。

2.知识点、奖学金、GPA的设定

具有特色的RUCRICH机制：知识点相对应于原版大富翁的金币，具有购地、升级、交费的作用；奖学金对应与原版大富翁的点券，具有购买道具卡的作用；GPA是RUCRICH的独创机制，GPA的大小将影响彼此之间收取费用的利率，并在特定的地点可以用知识点换取GPA。

3.移动功能

动态显示的移动：玩家的移动将有掷出的骰子点数决定，每回合玩家掷出一颗骰子，点数为1—6，并在游戏界面中动态显示掷骰子的过程，玩家移动相应的步数，玩家的移动并不是简单的平移，而是有走路的动态效果。

功能的扩展：实现多枚骰子的同时投掷。

4.购地功能

购地：玩家到达无人拥有的地皮，玩家可选择要不要购买。选择购买后，该地皮将为该玩家所属，并有特殊的标记。

5.房产升级功能

房产升级：当玩家再次走到自己购买的地皮上时，可以选择是否进行升级。升级需要一定的费用，同时升级后的地皮也将收取更多的过路费。地皮共可升级5次，每个等级都有不同的房屋显示，升到最高级后，将会触发游戏的彩蛋。

6.收取费用功能

费用收取：当一名玩家走到另一名玩家的地皮上时，要付给另一名玩家过路费（知识点）。过路费（知识点）的多少由房子的等级和双方的GPA大小决定。拥有地皮的玩家获得路过玩家的知识点。

7.道具卡片功能

道具卡片：RUCRICH共有八种卡片，具有各自的功能，当卡片使用完后，可到特定的商店花费奖学金进行补充，八中卡片分别为：
卡绩点：选择放到地图上任意一个，下一个角色经过该地时将被强制停下。
调分卡：选择任意一处已经被购买的地产，可对其进行升级。
挂科卡：选择任意一处有房子的地产，降低其等级。
一卡通：控制下一轮骰子的数字。
考试周：指定一名角色，令其立即入狱3天。
拖堂卡：令使用该卡的角色此回合停留一回合。
叶澄海楼：强制购买此时该角色所在的房产。
偷笔记：自己增加20%的知识点，对方减少20%的知识点。

8.多功能设施用地功能

多功能设施用地：每一块多功能设施用地在地图上占两个位置，当无人购买时，该地与普通地皮相同。该地皮可以选择五种不同的建筑，分别如下：
公园：没有任何用处和功能。
研究所：共可升级4次，随着等级的不同，玩家每次经过此地时，获取不同的功能卡片。
旅馆：共可升级4次，随着等级的不同，另一名玩家经过此地时，缴纳不同的过路费（知识点）。
商店：共可升级4次，随着等级的不同，另一名玩家经过此地时，缴纳不同的过路费（知识点）。
体育馆：共可升级4次，随着等级的不同，另一名玩家经过此地时，扣除响应比例的GPA。

9.入狱功能

入狱：当玩家被另一名玩家使用考试周或触发随机事件不幸入狱时，玩家进入监狱，并显示进入监狱的动画。进入监狱后，不可移动，不可收租盖房子。

10.交易功能

交易：玩家在两个地点能够通过奖学金交换功能卡片，能用知识点交换GPA。

11.地图显示功能

地图显示：地图上的每个地点都有相对应的人大地点名称，点击相应的地方，地图上将显示该地方的美丽风景。

12.胜利条件

当一名玩家的知识点为0或负值时，该玩家破产，另一名玩家胜利。

功能的扩展：RUCRICH1.0版本只允许两名玩家同时参与游戏，后面将会添加自定义游戏人数的功能。
