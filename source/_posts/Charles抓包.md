---
title: Charles抓包
---

### 下载地址
Charles下载地址：[https://www.charlesproxy.com/latest-release/download.do](https://www.charlesproxy.com/latest-release/download.do)
下载解压，即可安装成功

### APP抓包

### 配置
```
- 1、点击顶部菜单栏【Help】–>选择【SSL Proxying】，点击【install Charles Root Certificate 】安装Charles根证书即可；
  证书安装一直下一步就可以。
- 2、点击【Proxy】–>【SSL Proxying Settings…】
- 3、在弹出选项卡中，勾选【Enable SSL Proxying】点击【add】。
- 在Host输入【*】表示接收任何主机，在Prot输入【443】最后点击【ok】保存****
- 4、点击【proxy】，取消选中window proxy
- 5、证书导入手机中
  - 1、点击顶部菜单栏【Help】–>选择【SSL Proxying】，点击【save Charles Root Certificate】安装Charles根证书即可。保存文件类型选择cer保存，文件名随便（例如123），然后传到手机上； 
  - 2、手机打开设置->安全->更多安全设置->加密和凭据->从存储设备安装（后续安装后，就会在用户平凭据中看到），然后选择刚刚下载的凭据加入，文件名选择自己知道
  - 3、如果不用，需要取消WLAN的高级选项为【无】
- 6、选中WLAN，长按连接的WALN，选择【修改网络】。高级选项，代理选择【手动】。输入服务器主机名-->电脑的ip地址(172.18.10.70)、服务器端口号（8888）--> （点击【Proxy】–>【Proxy Settings】我们在设置下端口号，默认即可，具体视自己电脑环境设置）

```

开始打开手机调试把，监听到对应的地址