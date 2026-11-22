# 鹏友助手（XPHelper）

<div align="center">
  <img src="icon_work/brand/about_logo.png" width="100" height="100" alt=XP-ApkHelper Logo">
  <h3>面向小鹏车机的管理与文件传输工具</h3>

  [![Version](https://img.shields.io/badge/version-2.0-1677ff.svg?style=flat-square)](#-当前版本)
  [![License](https://img.shields.io/badge/license-GPL--3.0-green.svg?style=flat-square)](LICENSE)
</div>

## 功能

- 查看安装和删除下载目录里的APK；也支持从手机或电脑网页上传APK  
- 车辆车机界面，支持夜间黑夜模式自动切换  
- 集成车机调试模式、检查模式、大屏诊断模式
- 实时显示ADB、TCP和OTA状态。可暂停或恢复OTA更新  

<img width="2400" height="1200" alt="screenshot-202611220303" src="https://github.com/user-attachments/assets/daf99c5a-4295-4b13-b1f7-bb848b96a91b" />  


<img width="2400" height="1200" alt="screenshot-202611212337" src="https://github.com/user-attachments/assets/9c7719ae-6d5f-4bc7-ab72-20ad9cde61d3" />  


## 下载与安装

打开车辆的ADB功能。从 [GitHub Releases](https://github.com/Kasugano-Soras/XPHelper/releases) 下载 APK，放入车机 Download 目录后，在ADB窗口输入
```shell
am start -n com.android.packageinstaller/.PackageInstallerActivity  -a android.intent.action.VIEW   -d "file:///sdcard/Download/XPHelper-2.0.apk"   -t "application/vnd.android.package-archive"   --user 0
```
车机会弹出确认安装选项  

<img width="2400" height="1200" alt="install-v22" src="https://github.com/user-attachments/assets/3e78bce9-8a5c-4151-b992-51d400f09049" />  

选择继续，安装完成后点击打开，根据提示授予ADB权限后即可使用。  

## 兼容性  

软件在小鹏 P7（SA8295P）焕芯版上测试通过，车机软件版本为天玑XOS 5.10.6.8902  

理论上支持所有搭载天玑XOS 5系统的大屏使用  

## 免责声明  

所有操作均应在车辆处于停车状态时进行。  
本软件是作者为在自有车辆上开展研究而开发的第三方工具，不对其兼容性和稳定性作出保证。
本软件与小鹏官方无关，其所实现的功能不代表已获得厂商认可。  
使用调试入口或安装第三方 APK 前，请确保已充分了解相关操作的影响及可能产生的后果。调试授权、安装第三方应用及其他改变车机行为的操作均存在一定风险，由此产生的后果由使用者自行承担。
