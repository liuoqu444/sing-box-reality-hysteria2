# 简介
- Reality Hysteria2 vmess ws一键安装脚本
  
## 功能

- 无脑回车一键安装或者自定义安装
- 完全无需域名，使用自签证书部署hy2，使用cloudflared tunnel支持vmess ws优选ip
- 支持修改reality端口号和域名，hysteria2端口号
- 无脑生成sing-box，clash-meta，v2rayN，nekoray等通用链接格式

## 需求

- Linux operating system
- Bash shell
- Internet connection

## 使用教程

### reality和hysteria2 wss三合一脚本
```bash
bash <(curl -fsSL https://github.com/liuoqu444/sing-box-reality-hysteria2/raw/main/reality_hy2_ws.sh)
```


|项目||
|:--|:--|
|程序|**/root/sbox/sing-box**|
|服务端配置|**/root/sbox/sbconfig_server.json**|
|重启|`systemctl restart sing-box`|
|状态|`systemctl status sing-box`|
|查看日志|`journalctl -u sing-box -o cat -e`|
|实时日志|`journalctl -u sing-box -o cat -f`|

warp解锁v4 v6等操作自行使用warp-go脚本
具体操作就不说了
```
wget -N https://gitlab.com/fscarmen/warp/-/raw/main/warp-go.sh && bash warp-go.sh
```

## Credit
- [sing-reality-box](https://github.com/deathline94/sing-REALITY-Box)
- [sing-box](https://github.com/SagerNet/sing-box)
