---
title: Ngnix部署运行
---

### Ngnix下载
官方网站：[http://nginx.org/en/download.html](http://nginx.org/en/download.html)

### 启动Ngnix
- 直接双击nginx.exe，双击后一个黑色的弹窗一闪而过。
- 打开cmd命令窗口，切换到nginx目录下，输入命令 nginx.exe 或者 start nginx ，回车即可。

### 关闭nginx
如果使用cmd命令窗口启动nginx，关闭cmd窗口是不能结束nginx进程的，可使用两种方法关闭nginx
- 输入nginx命令 nginx -s stop(快速停止nginx) 或 nginx -s quit(完整有序的停止nginx)。
  
### 打包文件存放
- 文件放在html(D:\ngnix\nginx-1.22.1\nginx-1.22.1\html)
- nginx.conf下修改配置文件 root文件存放位置 listen端口
- 运行localhost:listen端口(http://localhost:90)