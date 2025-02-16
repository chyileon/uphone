## 功能相关
### Q:云手机跟云游戏有什么区别？

>A:云游戏是云手机的一个特殊应用场景，其最终面向的是游戏玩家，因玩家对游戏体验的苛刻要求，需要满足低延迟20ms以内、帧率稳定30或60帧、高画质720p以上、高码率4M以上等特点，需要全国覆盖的机房、高性能的云手机、抗弱网抖动流媒体传输、每路游戏需要至少4Mbps带宽。了解UCloud云游戏产品请转：https://docs.ucloud.cn/ugame/README

>云手机的普通应用场景包括游戏辅助、私域流量、跨境电商和RPA自动化等，这些普通场景主要面向企业、工作室、个人，侧重于功能实现、防封技术等，而对延迟、帧率、画质、抗弱网、带宽需求并不高。


### Q:相同的价格，在其他厂商可买到2-3核的手机，在UCloud为何只能买到1核的？

>A:其他友商采用SoC架构云手机，CPU虽然是8核，但可能是大小核模式，如1个Cortex A77 3.1GHz+3个Cortex A77 2.42GHz+4个Cortex A55 1.8GHz，或者是2个Cortex-A72 2.0GHZ+4个Cortex-A53 1.5GHZ小核； 另外在GPU功率过高发烫时CPU也可能降频，导致掉帧、卡顿的出现，甚至最高只能到55帧，无法达到原神的60帧体验。
  
>而UCloud云手机基于服务器架构，CPU核数全部为3.0GHZ的大核，没有小核，跑小游戏龙与王者占用0.2核CPU，跑王者荣耀只占用0.4核，跑原神也刚刚1核，所以3核以内规格足以胜任所有大中型游戏。在服务器上，显卡的PCIe总线带宽可以达到100Gbps，NVME盘可以达到16Gbps吞吐，在鲁大师跑分中，UCloud云手机（4大核+8G服务器DDR4内存+服务器显卡+NVME存储）以146万分排第一，比第二名黑鲨4S Pro（8核16G）高40万分。所以，SoC架构同等核数的云手机只能望其项背，无法相提并论。

### Q:UCloud云手机安卓版本是多少， 是否支持安卓11.0版本？

>A:目前是安卓AOSP 9.0版本，暂不支持11.0版本，安卓应用一般都支持多种版本的SDK，安卓版本对APP影响并不太大，如有刚需可反馈给客户经理，我们进行跟进。


### Q:云手机支持TikTok应用吗？

>A:目前可以运行TikTok，暂时还不支持摄像头推流直播。直播可以用PC机+ UCloud UDPN国际加速方案，详情请联系客户经理。



### Q:云手机支持一键新机吗？

>A:支持，每台云手机在创建时会自动生成设备的唯一信息，目前已增加13种机型，后续将继续增加机型。目前已经支持的参数见表格：
>![企业微信截图_c484768e-000d-4970-8b20-9a751e0c04e2](https://user-images.githubusercontent.com/5512170/173987073-c4862c1d-6948-402a-80ae-884a60a0ae7f.png)
![企业微信截图_ce71226a-9c8e-4c68-b73d-6ab4941ec54f](https://user-images.githubusercontent.com/5512170/173987051-f6fdd8ec-3029-4447-86bd-44b97f3019cc.png)


### Q:云手机支持独立IP吗？

>A:支持，IP地域可选华北一、上海、广州、香港、台北、日韩、东南亚和欧美，为降低成本，1个IP也可以给多部手机共用

### Q:云手机群控功能支持分给子账号吗？

>A:可以在不同项目中对云手机进行分类管理，可以给云手机划分不同的业务组，主账号可以在访问控制中调整项目/子账号的权限


## 体验相关

### 如何用客户端连接云手机？

>目前暂未推出正式的安卓和IOS 客户端，可以先用二维码中的客户端Demo进行简单连接操作
>操作步骤：
>1. 从控制台获取云手机的“资源ID”   2. 在客户端Demo的云手机里输入“资源ID” 即可连接
>
><img width="442" alt="云游戏体验版" src="https://user-images.githubusercontent.com/5512170/174747334-1b3c3a11-2830-427e-b553-b81f88af1536.png">

### 客户端看带宽有时2Mbps，有时几十百Kbps，是不稳定吗？
> 这是正常的，webrtc有动态码率能力，画面静止或变化少时传输量会减少、带宽占用低， 如果画面巨大变化时带宽仍然非常低是不正常的。

### 每路云手机给2Mbps带宽够用吗？能带的动吗？
> 没有问题，视频流给多少带宽和码率都可以，码率低只会影响清晰度，不影响卡顿和流畅度。

### 如何体验下云游戏的效果？
> 下载上述二维码的客户端，点击游戏图标即可体验。 注：演示服务器在杭州，不同地域的玩家到杭州延迟会有差异
> H5体验：拷贝地址到手机微信或者浏览器  https://www.ugame.ucloud.cn/mobile/index.html#/

### 安装APP时提示”解析软件包出现问题“或”应用未安装“ 怎么解决？
>  <img width="294" alt="企业微信截图_5accb9aa-e1b9-48d0-b127-c00e320edce5" src="https://user-images.githubusercontent.com/5512170/175291960-27dc20cf-72aa-4e18-9fdd-5c7345200dc7.png">

>  这种情况大多发生在小规格云手机安装大型APP，存储空间不足时会出现该现象，可以通过”设置->存储“ 查看剩余空间是否紧张，卸载不必要的APP或清理缓存空间，或购买更高规格的云手机。

### Q:如何体验更高画质的云手机？

>目前默认提供2M码率的画面带宽，如需要体验更高画质可单独调整云手机画面带宽


### Q:云手机内部网速慢怎么办？

>A:可以卸载掉不必要的APP，减少APP后台自动更新、下载等占用带宽；
   也可以根据需求量购买更大带宽，游戏类占用带宽较低，TikTok视频类每部手机需要0.5Mbps带宽，可以购买少量带宽给多部云手机错峰使用带宽来降低成本。
   
### Q:有的APP安装时间久是什么原因?

>A:很多大型APP安装时会执行dex2oat编译程序，完全占满所有分配的CPU，而不同规格限制了cpu的峰值，会拉长安装时间，但只出现在首次安装，后续使用时占用cpu很低，如王者荣耀 创世与魔法 梦幻西游正常玩时占用0.3核左右。

### Q：出现个别云手机无法连接怎么办？

>A:可关闭群控页面重新打开，或尝试重启云手机解决

### Q：有的游戏安装后闪退怎么办？

>A: 1.可尝试使用游戏官网的版本安装，TapTap和应用宝等渠道更改了包的信息，偶尔会存在兼容问题 2.可先尝试使用UCloud应用市场里的版本进行安装 3. 反馈给UCloud团队更新应用市场

<img width="307" alt="企业微信截图_fba41bda-6e11-436e-85d8-a19b0c299544" src="https://user-images.githubusercontent.com/5512170/175477681-04ae6190-2ae9-4759-ab91-ce651cb040b9.png">


### Q：抖音和TikTok、快手和部分APP刚开始启动时声音断断续续，看起来很卡？
>部分APP是在安装时执行dex2oat，表现为安装时间久；部分app（如抖音、TikTok、快手、微信、企业微信）是在安装后首次启动时执行dex2oat编译程序，dex2oat会把cpu全部占满，持续约几分钟，表现为声音断断续续、又像网络卡顿，后续使用时不再执行dex2oat，占用CPU也很少。

### Q：独立IP的共享带宽买多大合适？
>TikTok约占用0.5Mbps带宽，对于视频类APP可以2个云手机共用1Mbps；也可以通过错开时间段来使用共享带宽，比如20个手机买5M带宽，每天分2组每组10个同时播放视频；
>对于游戏类APP，其上报游戏数据量较小，可以10个云手机共用1M带宽进行配比；

## 二次开发
### Q:云手机管理的API文档在哪看？
> https://docs.ucloud.cn/api/uphone-api/README

### Q:云手机画面连接的SDK在哪下载？
> 目前是通过线下单独提供，请联系客户经理提供

### Q:是否支持ADB连接云手机？
> 整机服务器购买方式支持，零售方式暂不支持。可通过云手机服务器IP+端口号连接，每个手机一个端口号，正在开发中

### Q:ADB连接是否可以通过内网？
> 目前是通过公网进行连接，暂不支持内网连接方式

### Q:是否支持自定义安卓ROM？
> 目前可以基于UCloud标准的安卓镜像安装APP、更新Launcher、更换Logo和安卓机型参数来自定义安卓系统， 不支持源码级别的自定义。

### Q:是否支持xposed 谷歌三件套？
> 支持，标准镜像和TikTok镜像中自带谷歌三件套，未包含xposed

