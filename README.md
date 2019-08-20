### 松灵机器人（东莞）有限公司 UGV 产品固件升级说明文档

![scout](https://github.com/AglieX/agilex_firmware/blob/master/photos/SCOUT%E6%95%B4%E8%BD%A6.293.png)
---

#### 文件说明说明
- **cp210_drivers** 

   驱动板使用串口驱动文件
- **firmware_bin_files**
   + hunter

     UGV 产品 HUNTER 支持固件列表以及必要的说明文件
   + scout
    
     UGV 产品 SCOUT 支持固件列表以及必要的说明文件
- **firmware_upgrade_utility**

    固件升级工具

- **rs232_drivers**

    主板串口固件，不同型号支持不同，此驱动仅适配松灵产品通讯包配件所使用串口

---
#### 固件升级使用说明
- **准备工作**
    - 软件准备

       + 下载固件升级工具 firmware_upgrade_utility 

       + 下载车型所适配的固件 

       + 检查串口驱动已经正常安装，能否正常使用，具体可以通过设备管理器查看当前串口是否已经安装驱动
       ![设备管理器](https://github.com/AglieX/agilex_firmware/blob/master/photos/%E8%AE%BE%E5%A4%87%E7%AE%A1%E7%90%86%E5%99%A8.png)

    - 硬件准备（整车固件升级）

       + 串口DB9口连接至底盘上DB9接口，此时整车未上电

- **软件升级**
   - 打开firmware_upgrade_utility 软件，如下午所示,**波特率以及其他相关参数已经预置，不需要客户自行设置**，端口号如果驱动已经正常安装，端口好会自动读取，不需要客户自行选择
   ![升级固件工具](https://github.com/AglieX/agilex_firmware/blob/master/photos/%E5%8D%87%E7%BA%A7%E8%BD%AF%E4%BB%B6.png)
   
   - 点击开始连接按钮

   - 立即给SCOUT/HUNtER 底盘上电即可，连接成功后，可以显示当前机器人版本号，在升级前建议记录此版本号，以免在发生未知情况时可正常回滚

   - 点击**加载文件**按钮，选择需要升级的固件

   - 点击**开始升级**

   - 若升级成功，会提示升级完成提示框。

   - 断电重启即可。
---

### 常见问题与解决
 1. 点击开始连接以后，显示**连接超时**无法连接？

 - 检查串口的连接是否可靠，检查串口与UGV底盘面板处连接是否可靠，确认已经连接正常
 - 检查电脑上是否同时挂载了多个串口设备导致COM 读取错误
 - 无法解决可以联系 support@agilex.ai

 2. 连接正常，但是点击**开始升级**以后，进度条一开始正常，然后卡住不动了
 - 可能的原因的传输出现了异常，建议重新建立连接，再次下载。
 ---


    