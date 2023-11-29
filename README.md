# better-cloudflare-ip

查找适合自己当前网络环境的优选Cloudflare Anycast IP

## 用户数据安全声明

此版本不需要用户上传任何数据到服务器，服务器仅提供IP地址池维护以及下发！

## 用户自定义数据

用户可自定义ips-v4.txt和ips-v6.txt的IP地址段，如果使用数据更新将会覆盖本地自定义的数据

自定义ips-v4.txt的内容格式为 x.x.x.x或者x.x.x.x/x的CIDR写法，默认提取.前三位

自定义ips-v6.txt的内容格式为 x:x:x:x:x:x:x:x或者x:x:x:x:x:x:x:x/x的CIDR写法，默认提取:前三位

更多自定义玩法待用户自己发现

## Linux版本only

完整复制下方链接粘贴到控制台并回车，后续运行只需输入./cf.sh并回车即可

目前已经测试 Termux、OpenWrt、Ubuntu、Debian、CentOS、MacOS、Raspbian、Armbian、iSH

``` bash
curl https://raw.githubusercontent.com/badafans/better-cloudflare-ip/master/shell/cf.sh -o cf.sh && chmod +x cf.sh && ./cf.sh
```

## 引用声明

对于 Cloudflare ASN https://bgp.he.net/AS13335 ，Cloudflare IP Ranges 来自 https://www.cloudflare.com/zh-cn/ips/
