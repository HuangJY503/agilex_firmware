### AgileX Robotics (Dongguan) UGV Product Firmware 

![AgileX robotics product view](https://github.com/agilexrobotics/agilex_firmware/blob/master/photos/%E4%BA%A7%E5%93%81%E7%9F%A9%E9%98%B5.png)
---

- For chinese version help document please view![中文版本说明](https://github.com/agilexrobotics/agilex_firmware/blob/master/README_CN.md)

--- 


#### Drivers Document
- **cp210_drivers**

    USB to RS232 serial  for windows system drivers files

- **Firmware bin files**
    + HUNTER

    HUNTER supported firmware list and necessary documentation
    + SCOUT MINI 
    + SCOUT 1.0
    + SCOUT 2.0

    SCOUT supported firmware list and necessary documentation

    + TRACER
    + BUNKER

#### Firmware upgrade instructions
- **Prepare Work**
    -  Software preparation

        + Download firmware upgrade tool firmware_upgrade_utility
        + Download the firmware for the model, confirm the hardware currently in use, the product has been continuously optimized, and some accessories require corresponding configuration to support.
        +  Check whether the serial port driver has been installed normally and whether it can be used normally. You can check whether the current serial port has a driver installed in the device manager.
        ![Device management](https://github.com/agilexrobotics/agilex_firmware/blob/master/photos/device_manager.png)
    - Hardware preparation
        
        + The serial port DB9 port is connected to the DB9 port on the chassis, and the robot is not powered on at this time.

- **Firmware upgrade** 
    -    Turn on the firmware_upgrade_utility software, as shown in the figure below,**the baud rate and other related parameters have been preset and do not need to be set by the customer**. If the driver has been installed normally, the port number will be automatically read.
    photos/%E5%8D%87%E7%BA%A7%E8%BD%AF%E4%BB%B6.png)
    ![Firmware upgraade software tools](https://github.com/agilexrobotics/agilex_firmware/blob/master/photos/%E5%8D%87%E7%BA%A7%E8%BD%AF%E4%BB%B6_EN.png)

    + For customers who use the USB to RS232 cable, choose **USB to RS232** in the **upgrade tool**.
    + Then select the appropriate **COM port**.
    + Click the start connection button.
    + Power on therobot immediately. After the connection is successful, the current robot version number can be displayed. It is recommended to record this version number before upgrading to avoid normal rollback in the event of unknown circumstances.
    + Click the Load File button and select the firmware to be upgraded.
    + Click to start upgrade.
    + If the upgrade is successful, it will prompt the upgrade completion prompt box.
    + Power off and restart.

###  Questions and Solutions
1. After clicking start to connect, it shows that the connection timeout cannot connect?

    - Check whether the connection of the serial port is reliable, check whether the connection between the serial port and the UGV chassis panel is reliable, and confirm that the connection is normal.
    - Check whether multiple serial devices are mounted on the computer at the same time and causing COM read errors.
    -  If you can’t solve it, please contact support@agilex.ai.

2. The connection is normal, but after clicking to start the upgrade, the progress bar is normal at first, and then stuck.
    
    -  The possible reason is that the transmission is abnormal. It is recommended to re-establish the connection and download again.