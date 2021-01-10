# 新路由3（Newifi-D2）自动编译最新版OpenWrt（Lede）

*每24小时自动编译一次，在Action中下载*

## 编译特性
- 默认主题为argon
- 默认使用开源WIFI驱动（支持802.11kvr）
- 默认启用helloworld
- 外挂存储支持格式exfat, ntfs, ext4

## 插件列表（下表内容待完善，具体请以编译配置文件为准）

| 插件名                  | 说明               |
| ---------------------- | ----------------- | 
| ~~aliddns~~                | 阿里云DDNS         |  
| aria2                  | Aria2下载工具       |
| frpc/frps              | 内网穿透客户端/服务端 |
| hd-idle                | 硬盘休眠            |
| ~~openvpn/openvpn-server~~ | OpenVPN客户端/服务端 |
| samba                  | Samba文件共享       |
| ttyd                   | 网页终端            |
| xlnetacc               | 迅雷快鸟            |
| helloworld             | -                  |


*如需多拨功能，请在`.github/workflows/NEWIFI-D2.yml`文件`# 常用LuCI插件选择:`中的 `cat >> .config <<EOF`行下方增加以下三行
```
CONFIG_PACKAGE_luci-app-mwan3=y
CONFIG_PACKAGE_luci-app-mwan3helper=y
CONFIG_PACKAGE_luci-app-syncdial=y
```
## 网关地址
- IP 192.168.1.1
- Username root
- Password password

## Credits
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
- [KFERMercer/OpenWrt-CI](https://github.com/KFERMercer/OpenWrt-CI)
