# Modbus云网关

| 产品图                                                       | 产品介绍                                                     |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| ![image-20191028180054605](README.assets/image-20191028180054605.png) | Modbus云网关是基于物联网边缘计算应用开发框架[FreeIOE](https://github.com/freeioe/freeioe)项目精心定制的一款Modbus设备数据上云专用网关，<br/>这款网关采用国产ARM A7 4*Core CPU + openwrt操作系统 + 边缘计算应用框架 FreeIOE 定制版的技术方案，<br/>提供 2 路以太网（10M/100M自适应）和 2 路串口（1 * RS232/2 * RS485），<br/>并结合云配置/云运维的方式为工业物联网用户提供 Modbus 设备一键上云的极致体验。 |





## 主要特性

* __超强计算性能__
  
  arm-A7 4核CPU 主频高达1GB MHz,配合 256MB 大内存，超强性能轻松应对海量数据采集加工转发。
  4GB eMMC 存储介质，数据缓存还是本地数据存储分析，安装运行更多程序，也毫不畏惧。
  专为工业物联网边缘应用设计，是设备侧边缘计算的最佳选择     
  <br/>
  
* __规整小巧的结构设计__
  
  采用合金壳体，内部使用专业散热考量，两侧蜂窝眼设计，即可保证优良的散热性能，又能提供坚固强劲的机身。
  规整的外观及小巧的尺寸(120mm \* 95mm \* 30mm)，很容易在受限空间中找到位置。    
<br/>
  
* __灵活的安装方式__
  
  DIN导轨安装<br/>
  壁挂安装
<br/>
  
* __全面的隔离保护__
  
  整机保护——电磁兼容试验和测量技术脉冲磁场抗扰度试验- GB/T 17626
        【
            GB/T 17626.2-2006 静电放电抗扰度 3级
            GB/T 17626.3-2006 射频电磁场辐射抗扰度 3级
            GB/T 17626.4-2006 电快速瞬变脉冲群抗扰度 3级
            GB/T 17626.5-2006 浪涌（冲击）抗扰度 3级
            GB/T 17626.6-2006 射频场感应的传导骚扰抗扰度 3级
            GB/T 17626.8-2006 工频磁场抗扰度 3级
            GB/T 17626.9-2006 脉冲磁场抗扰度 3级
        】
  串口隔离保护——RS485/RS422不仅具有正负15K∨的抗静电干扰，而且具有3750Vrms的接口隔离，即在RS485线和外壳之间加3750V交流电压，漏电到网关内部电流小于5mA.。完整的保护方案能使RS-232/RS-485设备安装于仼何复杂的工业环境而免除静电、雷击、电磁和浪涌对设备的干扰或损坏。串口隔离模块是工业级电流信号隔离分配器，采用磁隔离技术保证隔离器的隔离功能：输入、输出、电源之间全隔离，能够屏蔽现场各种干扰信号和有害信号，同时保证输岀信号不衰减，提供高精度信号，提高系统可靠性。<br/>
  网络隔离保护——网口提供2KV级浪涌保护，隔离来自网口的破坏信号。<br/>
  机壳保护——整机具有高强度抗电磁干扰，外壳采用抗辐射的SECC板，提供外壳接地端子，可以将雷击电流释放到大地，保护产品。
<br/>
  
* __强悍的RS485负载能力__
  
  RS485具有驱动最高可达128个负载的能力，和驱动32个负载的产品相比，可以实现更多设备数据连接能力，节约了成本。
<br/>
  
* __2路独立 10M/100M 自适应高品质网口__
  
  2路独立 10M/100M 自适应网口，通过配置，可灵活的选择交换模式，路由模式。
<br/>
  
* __高品质接线端子__
  
  5.08间距快捷安装插拔组合， 安装牢固、便捷、稳如泰山。主要应用于自动化电气连接系统，缩短接线时间，提高接线效率。<br/>
  绝缘件：PA66阻燃等级∨0 | 压线框；铜质压线框镀镍 | 导电件：磷青铜镀锡抗氧化性强 | 螺丝：铁螺丝镀锌或锡
  <br/>


* __4G全网通__
  
  移动/联通/电信自动适配，同时支持用户自定义接入专用APN。
<br/>
  
* __备电模块（选配）__
  
  最大10000mah的电量让网关无外部供电也可续航20小时，实时侦测现场电源故障从容发出告警等处理。
<br/>
  
* __不限设备数量__
  
  网关软件功能上未限制设备数量，让你使用时无后顾之忧。
<br/>
  
* __不限设备点数__
  
  网关软件功能上未限制设备点数，采集设备数据时一个点都不要放过。
<br/>
  
* __4GB存储空间__
  
  4GB的存储空间，即可实现数据的缓存，也可通过[FreeIOE社区](https://freeioe.org)扩展更多应用功能
<br/>
  
* __云端设备模板__
  
  云端提供大量的设备模板，你即可一键采集设备数据，还可以自行创建编辑，又可分享给他人共用
<br/>
  
* __设备配置云端备份/恢复__
  
  云端提供设备配置的多个版本，你可一键恢复历史版本，也可更换网关时一键恢复网关配置。
<br/>
  
* __Modbus RTU/ASCII/TCP全覆盖__
  
  Modbus RTU/ASCII/TCP 完全覆盖，支持 RTU over 以太网/ASCII over 以太网，即使是Modbus协议的非标准使用，也可在[FreeIOE社区](https://freeioe.org)找到完美方案。
<br/>
  
* __MQTT上云__
  
  设备数据，设备事件，设备报警，等等一键上云；还可支持数据下置反向控制设备。整个过程支持全面的加密及验证。
<br/>
  
* __数据缓存__
  
  网络不稳定，服务器需要升级，这些情况如何保证数据完整性？<br/>
  完全不需担心！MQTT上云支持数据缓存，3.5GB的存储空间让你长时间断网也不担心数据丢失。
<br/>
  
* __数据全面加密压缩传输__
  
  MQTT上云通道完全支持SSL/TLS加密及用户ID等认证，不惧网络监听；高效的数据压缩，节省流量最高可达10倍。
<br/>
  
* __有线/无线自适应__
  
  同时支持有线/无线连接互联网，互为冗余，并可根据需要优先选择指定链路。
<br/>
  
* __基于开源路由系统OPENWRT定制__
  
  基于开源路由系统OPENWRT定制，定期升级最新版本修复系统安全漏洞，减少网络黑客攻击的危害，还可通过社区获得更多实用的应用功能和安全防护，让网关无限可能。
<br/>
  
* __一套专为工业物联网平台量身定做的平台型智能应用网关，提供全功能REST API__ 
  
  通过云平台，可以管理在任何地方的网关，网关所有的功能及操作都可通过云平台完成。REST API让网关管理运维功能和你的业务系统无缝集成。
  <br/>
  
* __实时感知，网关离线和现场设备掉线/宕机__
  
  网关和设备之间，网关和平台之间，设计了心跳机制，因此设备故障或离线，网关故障或离线，平台都可感知。 <br/>