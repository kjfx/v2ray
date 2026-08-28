# V2ray搭建教程，vps搭建v2ray方法，vpn搭建v2ray 一键搭建代码
V2ray搭建视频教程：▶ https://youtu.be/T5ZIAU9K2Do
### 步骤：<br>
**1、Vultr注册账号**：https://www.vultr.com/?ref=9827682<br>

**2、选择服务器**<br>

**3、打开搭建工具 FinalShell**<br>
FinalShell：[点击下载>>](https://kjfx.lanzoui.com/iqm6Uosbzha)<br>
备用下载（含MAC版）：<a href="http://www.hostbuf.com/t/988.html" target="_blank">点击下载>></a><br>

**4、V2Ray一键安装代码**<br>

    bash <(curl -s -L https://git.io/v2ray-setup.sh)

<br>

    #放行端口
    iptables -I INPUT -p tcp --dport 80 -j ACCEPT
    iptables -I INPUT -p tcp --dport 8080 -j ACCEPT

BBR加速

    echo "net.core.default_qdisc=fq" >> /etc/sysctl.conf
    echo "net.ipv4.tcp_congestion_control=bbr" >> /etc/sysctl.conf
    sysctl -p

**5、科学上网软件下载**<br>
软件下载：https://github.com/Kejifaxian/welcome<br><br>

<hr/>

## Vultr网站界面更新了，以下是快速入口和选择说明
注册账号：https://www.vultr.com/?ref=9827682<br>
充值入口：https://console.vultr.com/billing/<br>
个人信息：https://console.vultr.com/user/profile/<br>
购买服务器入口：https://console.vultr.com/deploy-beta/<br><br>

<img src="https://raw.githubusercontent.com/kjfx/v2ray1/refs/heads/main/vps%E6%9C%8D%E5%8A%A1%E5%99%A8%E9%80%89%E6%8B%A9%E8%AF%B4%E6%98%8E.png" />

