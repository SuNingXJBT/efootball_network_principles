Telegram group channel: https://t.me/efootballCheaterReport

Telegram group: https://t.me/eFootballxjbt

相关工具在 QQ群143552766 分享

Network Principles of Konami eFootball PES

>The server domain used for game login and user data management is pes22-game.cs.konami.net. All servers are hosted on AWS in Portland, USA. The DNS updates with different sets of IPs every few minutes.

>The update server domain is d1ln4m3c7n87ju.cloudfront.net. It is globally distributed, with DNS refreshing every few minutes, and each time eight servers in a region become active.

>Access to the above servers works similarly to browsing web pages. Using a stable proxy can ensure game stability and avoid disconnections.

>Matchmaking servers are distributed across more than 50 regions worldwide, primarily using Google Cloud, with AWS as a supplement.

>The game continuously pings speed test servers in various regions, and the results determine where subsequent matches take place.

>Matchmaking modes are divided into Peer-to-Peer (P2P) and Client-Server (relay) modes. Friendly matches use P2P, while the vast majority of other matches use Client-Server.

>In Client-Server mode, the player's gaming experience depends entirely on the network quality between themselves and the server, and is unrelated to the opponent's network conditions. Moreover, the servers are stable most of the time; any instability experienced by a player is due to network issues between themselves and the server.

>Client-Server mode also includes both UDP and TCP connections. If TCP is used, even sitting directly on the server will result in noticeable latency. Frequent stuttering or fast-forwarding in-game is mostly caused by TCP mode.

The above summarizes the network principles of Konami eFootball PES — very simple and easy to understand. Based on these principles, solutions to common in-game network issues are also straightforward.

1. Login restriction error CODE::C_GKCC_0019, or disconnection prompts during gameplay

>When accessing the game server pes22-game.cs.konami.net, an access region check is performed. To bypass this check, simply use a proxy from an unrestricted region. If setting a global proxy affects other operations on your computer, you can use Proxifier or Netch to handle network access only for efootball.exe. In the PES era, this method was referred to by some groups as "Method One".

>During matches, players also continuously interact with this data server to record yellow/red cards, scores, and other information. For Chinese players, stable access to any IP under this domain is not guaranteed. Network instability, or a DNS update that points to an IP unreachable from China, will inevitably result in match interruptions.

2. Update failures on Thursdays

>The GitHub project Thursday_Update_Helper contains detailed step-by-step instructions.

>You need to resolve connectivity issues with the update server d1ln4m3c7n87ju.cloudfront.net. Using a proxy is one solution.

>Every few minutes, the DNS updates the IP group for this domain. Different DNS servers may return different resolution results at the same time, so you can try switching DNS servers to attempt different IPs for the update.

>Using local DNS resolution to point the update server to an idle IP can improve update success rates.

3. Pros and cons of P2P vs. Client-Server

>Opinions on this vary. Players can compare the network performance between friendly matches and ranked matches to draw their own conclusions. Those who can sit on the server won't want P2P.

>In P2P mode, match quality depends on the network between both parties and affects each other. However, generally speaking, both sides share a consistent experience — if the game lags, both will lag together.

>In Client-Server mode, the gameplay experience depends entirely on the network conditions between you and the server. It is not affected by the opponent, but it almost becomes a competition between both players' networks. If your network latency is more than 30ms higher than your opponent's, the two sides are essentially playing different games.

4. Persecution delusion

>In Client-Server mode, the gaming experience is not affected by the opponent. The network fluctuation graph also only reflects the condition between you and the server. Anyone claiming that the opponent is throttling them is experiencing persecution delusion.

5. Avoiding TCP mode matches

>The GitHub project eFootball_Block_TCP_Matches provides detailed descriptions. Simply put, you need to block TCP ports 5736 and 30000–35000.

科乐美eFootball实况足球游戏的网络原理

>用于游戏登录以及游戏中用户数据管理的服务器域名是 pes22-game.cs.konami.net 。 全部是在美国波特兰的亚马逊云。每隔几分钟，DNS会更新不同的IP组。

>更新服务器域名是 d1ln4m3c7n87ju.cloudfront.net 。 全球分布，DNS每隔几分钟刷新，每次有个区域八个服务器生效。

>以上服务器的访问方式类似于浏览网页，使用稳定的代理可以保证游戏的稳定性，避免断线。

>对战的服务器分布于全球50多个地区，谷歌云为主，亚马逊云为补充。

>游戏里持续对各地区的测速服务器测速，测速结果决定了后续对战发生在何处。

>对战模式分为点对点(peer-peer)和服务器中转(Client-Server)模式。友谊赛是点对点的，其他比赛绝大多数是服务器中转

>服务器中转模式(Client-Server)，玩家的游戏体验完全取决于自己与服务器之间的网络质量，与对手的网络情况无关。而且大部分时间，服务器是稳定的，玩家出现的不稳定状况是自己到服务器之间的网络问题。

>服务器中转模式也分为UDP和TCP链接两种。如果是TCP，即使是坐在服务器上，也会感觉到明显的延迟。游戏内如果经常出现停顿、快进，基本上是TCCP模式造成的。

以上就是科乐美eFootball实况足球游戏的网络原理，非常简单易懂。基于以上原理，游戏中常见的网络问题，解决办法也很简单。

1、登录受限提示 CODE::C_GKCC_0019， 游戏过程中出现断线提示
>  访问游戏服务器pes22-game.cs.konami.net时，会进行接入地区检查。为跳过该检查， 只要使用一个非限制区域的代理就行了。如果设置成全局代理的话，有可能影响电脑上其他操作。可以使用Proxifier或者Netch，仅针对efootball.exe程序的网络访问进行处理。PES时代，这个方法被某个群体称为方法一

> 在对战过程中，玩家也会继续和该数据服务器交互，记录红黄牌、比分等信息。对于中国玩家来说，并不能稳定访问该域名下任一IP。网络不稳定，或者DNS更新了一个中国玩家无法访问的IP，必然导致对战中断。

 2、每周四更新失败
>在github上Thursday_Update_Helper-项目里有详细的操作方法描述。

>需要解决与更新服务器 d1ln4m3c7n87ju.cloudfront.net 之间的链接问题，使用代理是方法之一。

>每隔几分钟，DNS会更新该域名的IP组，不同的DNS服务器，在同一时刻返回的解析结果是不一样的，可以更换DNS尝试不同的IP更新，

>使用本地域名解析将更新服务器指向空闲的IP，会提高更新的成功率

3、点对点和服务器中转的优劣
>这个问题的回答见仁见智，玩家自己比较一下友谊赛和天梯的网络差别，就能得出自己的结论。能坐在服务器上的玩家，是不会想要点对点的。

>点对点的对战效果取决于双方之间的网络，且会相互影响。但是大体来说，双方体验是一致的。比如要是游戏卡住的话，两边会一起卡住。

>服务器中转模式，游戏体验完全取决于自己与服务器之间的网络状况。不受对方影响，但几乎会成为双方网络的竞争。如果自己的网络比对手的延迟高出30毫秒以上，那两边几乎就是在玩不同的游戏了。

4、受迫害妄想症
> 服务器中转模式，游戏体验不受对方影响。网络波动图体现的也是自己和服务器之间的状况。 说对手在卡自己的，都是受迫害妄想症爆发。

5、避免TCP模式的对战
在github上eFootball_Block_TCP_Matches项目有详细描述， 简单说就是需要屏蔽5736以及30000-35000的TCP端口，


 
