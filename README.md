# VPN
Virtual Private Server

安装部署
=========================

**CentOS 6**
------

    wget https://raw.githubusercontent.com/XieXianbin/vpn/master/pptp/CentOS6-pptp-iptables.sh
    chmod +x ./CentOS6-pptp-iptables.sh
    ./CentOS6-pptp-iptables.sh -u your_username -p your_password

**CentOS 7 firewalld**
------

    wget https://raw.githubusercontent.com/XieXianbin/vpn/master/pptp/CentOS7-pptp-firewalld.sh
    chmod +x ./CentOS7-pptp-firewalld.sh
    ./CentOS7-pptp-firewalld.sh -u your_username -p your_password

**CentOS 7 iptables**
------

    wget https://raw.githubusercontent.com/XieXianbin/vpn/master/pptp/CentOS7-pptp-iptables.sh
    chmod +x ./CentOS7-pptp-iptables.sh
    ./CentOS7-pptp-iptables.sh -u your_username -p your_password

**Ubuntu**
------

    wget https://raw.githubusercontent.com/XieXianbin/vpn/master/pptp/Ubuntu-pptp.sh
    sudo bash Ubuntu-pptp.sh -u your_username -p your_password
    service pptpd restart


注意事项
==========

VPN 密码必须大于8个字符，否则脚本将自动生成一个随机密码。

可以在`/etc/ppp/chap-secrets`文件中添加更多账号。
