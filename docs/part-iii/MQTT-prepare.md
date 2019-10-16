## MQTT接收数据准备

### MQTT协议
[MQTT协议简介](https://wiki.freeioe.org/doku.php?id=mqtt:start)

### 安装MQTT Broker

本节内容以将网关的数据推送到自建MQTT服务器为例进行说明。

1) 自建MQTT Broker实际很简单，首先有一台互联网上可以访问的主机就可，这里我使用一台阿里云的ECS作为MQTT Broker服务器，然后再安装一个MQTT Broker软件即可，由于目前大多数物联网的平台都采用MQTT协议作为平台接入协议，因此各种MQTT Broker软件非常多，商业版本/免费版本/开源版本都有很多的选择，下面就是一张关于各种mqtt broker功能对比[https://github.com/mqtt/mqtt.github.io/wiki/server-support](https://github.com/mqtt/mqtt.github.io/wiki/server-support)，在本例中，我们采用国产的MQTT Broker [EMQ X Broker](https://www.emqx.io/cn/downloads#broker)，EMQ X Broker支持主流的各种操作系统Linux/Mac OS/Windows，这里我们选择Ubuntu/Linux版本，[按照官方安装指南](https://developer.emqx.io/docs/broker/v3/cn/install.html#ubuntu)非常容易的就将EMQ X Broker安装并运行起来了。EMQ X Broker自带WEB管理端，


2) 更改防火墙安全规则，开启MQTT Broker服务器的TCP端口，由于本例中使用了阿里云的ECS主机，默认情况下，MQTT Broker的服务端口并未在ECS主机的外部防火墙规则中开启，因此需要登录阿里云账户，在ECS主机的安全规则中开启MQTT Broker的服务端口，一般开启TCP端口1883，8883即可；如需要远程管理EMQ X Broker，可开启TCP端口18083；如前端页面需要直接访问EMQ X Broker，开启TCP端口8083，8084；更加详细的说明，可阅读EMQ X Broker的帮助文档。


### MQTT客户端
MQTT Broker完成安装后，可通过mqtt客户端工具测试一下EMQ X Broker工作是否正常，这里使用网上使用者较多的mqtt客户端工具[mqttfx](http://mqttfx.jensd.de/index.php/download),通过此客户端工具，能和自己部署的MQTT Broker收发消息，就说明工作正常了。下面继续说明如何在ThingsCloud平台配置ThingsLink网关，将ThingsLink网关的数据推送到自建的MQTT Broker。
