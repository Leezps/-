<h1>ShadowsocksR+搬瓦工=翻墙</h1>

> 对于一名程序员来说，会写代码的是程序员，但是不会Go Out Door的一定不是一名合格的程序员，今天我们来讲讲Go Out Door的那些事

**首先**

我们需准备两个东西，一个是ShadowsocksR，一个是搬瓦工的服务器（这个服务器要钱，所以不想给钱的我也帮不了你，但是可以给你个<a href="https://github.com/getlantern/forum">免费的Go Out Door软件</a>用用，但是每个月都有流量的限制，所以你规划好自己怎么使用），搬瓦工是国外的服务器，当然也有国内的网站，但是国内以前我也没用过，所以就不知道了什么流程，所以我这讲解的是如何从国外买了这服务器并且搭上ShadowsocksR进行Go Out Door

> (⊙o⊙)…既然有免费Go Out Door软件了，为什么还要服务器呢？因为这个服务器不仅可以Go Out Door，而且还可以搭建自己的博客网站、微信公众号的第三方后台等等，对于开发人员来说，好处多多…………（最重要的原因是你可以访问一些国外的视频网站( σ'ω')σ，其他的软件进行了限制，所以你可能会看不到，并且不用看别人软件的脸色，万一它要收费了，我们还要找新软件，而且麻烦）

**(既然好处多，我们就开始了)其次**

我们先安装一个<a href="https://github.com/getlantern/forum">蓝灯</a>，然后通过蓝灯访问guo外网，首先我们先去<a href="https://www.bwh1.net/">搬瓦工</a>官网租一台服务器，你可以租一台便宜的，每个月只需10多块，我相信你这点钱扣一扣还是给得起的，具体的租服务器的流程我就不说了，因为可以<a href="https://www.baidu.com/">百度</a>或者<a href="https://www.google.com/">Google</a>，说多了又感觉像打广告的了，推荐搬瓦工，是因为它便宜而且好…………

买了服务期之后，我们可以登录它的网站

第一步:

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_1.png"/>

第二步：

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_2.png"/>


第三步（你进入这样的一个界面）:

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_3.png"/>


第四步（找到我们的服务器）:

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_4.png"/>


第五步（进入服务器，并搭建好服务器端的SSR——ShadowsocksR）:

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_5.png"/>

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_6.png"/>


官方有一个比较好功能，就是一键搭建SSR,不需要我们具体配置之类的，当然这样的翻墙速度也就慢一些，如果你想要最优的，别人也给了<a href="https://233abc.com/post/8/">配置大法</a>的搭建完SSR，我们会发现我们有这么一个界面

<img width="1000px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_7.png"/>

这里面是关于官网对你的客户端的一些配置的讲解，（这儿只讲解windows的安装）我们将windows客服端下载下来之后，解压，解完压先别安装，我们**先来段基础知识**：

> XP默认并没有安装 .NET Framework v2.0和v4.0，需要手动安装，v4.0下载。

> Win7/8/10的系统一般都安装了 .NET Framework v2.0和v4.0 所以都能用。

> Mac请选择 ShadowsocksX-Mac-2.6.1.dmg（这个是Shadowsocks作者制作的，但是2015喝茶后已经不更新了，建议使用下面这三个）

> ShadowsocksX-R、ShadowsocksX-NG、GoAgentX-SSR.dmg（GoAgent的SSR插件）

**根据你系统安装 .NET Framework v2.0或4.0的支持库 来选择客户端中的 ShadowsocksR-dotnet2.0.exe 或 ShadowsocksR-dotnet4.0.exe 并打开客户端**

我们会发现电脑的右下角出现一个纸飞机的图标(估计你们的图标是白色，那是因为还没有配置SSR)：

<img width="500px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_8.png"/>

左击点开它

<img width="500px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_9.png"/>

在这里按照刚才服务器上提示的配置进行配置服务器的设置，然后就是就是修改如下几个地方：

(1)

<img width="500px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_10.png"/>

(2)

<img width="500px" src="https://github.com/Leezps/SSR-bandwagonhost-GoOutDoor/blob/master/banwagong/banwagon_img_11.png"/>


(3)将服务器负载均衡取消掉

**讲解为什么要选择系统代理模式为PAC模式与代理规则是绕过局域网和大陆？**

> 跳转国外网站SSR会经过两次判断

> 第一次判断是系统代理模式，**直连模式**不用讲就知道，它适合国外的电脑，因为直连的意思是不通过代理，直接访问该网站，但是我们与国外是断开的，所以直连根本就访问不到，**PAC规则**是根据PAC文件中的黑白地址名单来判断那些网站走代理，也就是判断 流量数据是进入SSR客户端还是直连，**全局模式**那就是全部都走代理，但是国内的网站我们可以直接访问得到，所以就不需要全部走代理了，我们就选择PAC模式

> 第二次判断是代理规则，如果上一次系统代理模式反馈的是需要使用代理，则跳到这个代理规则来，**绕过局域网**，局域网内IP 不走代理，局域网外IP 都走代理。**绕过局域网和大陆**，访问网站的是 大陆IP 都不走代理直连，访问 非大陆IP 的网站都走代理。**绕过局域网和非大陆**，访问网站的是 大陆IP 都走代理，访问 非大陆IP 的网站都不走代理，这个一般是海外访问国内网站用的。

好了，也没有什么讲的了，如果你SSR搭建的时候存在问题，可以通过<a href="https://doub.io/ss-jc39/">SSR基本问题</a>来解决，上面依旧没解决你搭建SSR的问题，欢迎留言

<h3>参考资料(有些资料需要翻墙才看得到，所以有可能你打不开)：</h3>

<a href="http://www.360doc.com/content/17/0523/18/33381298_656535600.shtml">SSR安卓端WIN电脑端使用教程及下载</a>

<a href="https://doub.io/ss-jc10/">ShadowsocksR 客户端 小白使用教程</a>

<a href="https://doub.io/ss-jc39/">Shadowsocks无法使用后的简单排除方法</a>

<a href="https://233abc.com/post/8/">SSR（ShadowsocksR）搭建和优化图文教程</a>
