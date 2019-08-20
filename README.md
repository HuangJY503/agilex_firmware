### 松灵机器人（东莞）有限公司 UGV 产品固件升级说明文档

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
   - 打开firmware_upgrade_utility 软件
   - 
    