## Modbus采集前期准备

### 连接物理设备
为使用Modbus Master应用和Modbus设备通讯时能更快更顺利的达到目标，我们有必要先了解及做一些准备工作。<br/>

1. 了解并确认Modbus设备具体是使用Modbus协议的哪一种子协议（Modbus RTU、Modbus ASCII、Modbus TCP）对外提供数据，一般来说，可以阅读设备提供的数据通讯类文档了解情况，还可以咨询设备的调试人员或者设备厂商的服务支持人员获得帮助。<br/>

2. 获取所有需要通讯的Modbus设备的物理链路信息，如是通过串口连接，需要知道Modbus设备串口的参数（波特率、数据位、停止位等信息），如是通过以太网连接，需要知道Modbus设备的IP地址及端口号。<br/>

3. 获取所有需要通讯的Modbus设备的Modbus设备地址信息，没有Modbus设备地址信息，无法进行后面的工作。<br/>

4. 获取Modbus设备对外提供变量数据的列表文件，一般来说，多少电子表格格式比较多，这种文件在自动化行业多称位设备点表，在这份点表中，我们可以看到设备的很多变量及其Modbus属性都会被罗列出来，一般会包含：名称、描述、Modbus功能码、Modbus寄存器地址、数据类型、运算系数等信息，如这份设备点表中无法获取到这些信息，那么就无法进行后面的工作。<br/>

5. 前面3个步骤的准备工作都完成后，还需要将Modbus设备提供点表整理为Modbus Master应用所需的点表，这个整理点表的工作通过电子表格软件（如Office EXCEL）可达到事半功倍的效果。Modbus Master应用的参考设备模板。<br/>

6. 确认网关和设备之间的物理连接是否正常，如是通过串口方式连接Modbus设备，检查串口接线是否正确；如是通过以太网方式连接Modbus设备，检查网线是否连接、网卡状态灯是否正常、还需要通过tcp/ip诊断工具检测是否可以连接到Modbus设备的IP地址（一般多使用ping命令）。<br/>


### 连接模拟软件
Modbus的仿真工具很多，使用符合标准的哪一种Modbus仿真工具都可以。可使用Modsim32 （[点击下载](http://thingscloud.oss-cn-beijing.aliyuncs.com/download/Modsim32.zip)）软件来模拟Modbus设备，作为配对的测试工具，modscan32是一个Modbus协议的验证工具。 查看[Modsim32快速使用](https://wiki.freeioe.org/doku.php?id=modbus:modsim32)。