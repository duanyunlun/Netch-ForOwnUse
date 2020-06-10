# Netch-ForOwnUse
[![Platform](https://img.shields.io/badge/platform-windows-orange.svg)](https://github.com/AmazingDM/Netch-ForOwnUse)
[![Version](https://img.shields.io/github/v/release/AmazingDM/Netch-ForOwnUse)](https://github.com/AmazingDM/Netch-ForOwnUse/releases)
[![Downloads](https://img.shields.io/github/downloads/AmazingDM/Netch-ForOwnUse/total.svg)](https://github.com/AmazingDM/Netch-ForOwnUse/releases)
[![Netch CI](https://github.com/AmazingDM/Netch-ForOwnUse/workflows/Netch%20CI/badge.svg)](https://github.com/AmazingDM/Netch-ForOwnUse/actions)
[![Pre Build CI](https://github.com/AmazingDM/Netch-ForOwnUse/workflows/Pre%20Build%20CI/badge.svg)](https://github.com/AmazingDM/Netch-ForOwnUse/actions)
[![License](https://img.shields.io/badge/license-MIT-yellow.svg)](LICENSE)
[![](https://img.shields.io/badge/Telegram-频道-blue)](https://t.me/Netch) [![](https://img.shields.io/badge/Telegram-讨论组-green)](https://t.me/Netch_Discuss_Group) 
[![Website](https://img.shields.io/website?url=https%3A%2F%2Fnetch.org)](https://netch.org/)

游戏加速工具

[网站](https://netch.org/)

## 相比原版Netch新增特性
- 进程白名单模式（全局）
- TCP UDP分流（支持Socks、SS、SSR、Trojan）
- 允许多开Netch（进程模式因驱动限制无法多开）
- 流量统计（如无bug将合并Netch主仓库）

## 进程模式进阶用法（原版有但是没写很多人不知道）

模糊匹配和全路径匹配

``` 
# test, 0
ntt.exe
Desktop
Desktop\NatTypeTester.exe
C:\Users\xxxx\Desktop\NatTypeTester.exe
```

## TOC
- [Netch](#Netch)
	- [TOC](#TOC)
	- [简介](#简介)
    - [新手入门](Quickstart.zh-CN.md)
    - [进阶用法](https://github.com/NormanBB/NetchMode/blob/master/docs/README.zh-CN.md)
	- [依赖](#依赖)
    - [语言支持](#语言支持)
    
## 简介
Netch 是一款 Windows 平台的开源游戏加速工具，Netch 可以实现类似 SocksCap64 那样的进程代理，也可以实现 SSTap 那样的全局 TUN/TAP 代理，和 Shadowsocks-Windows 那样的本地 Socks5，HTTP 和系统代理。至于连接至远程服务器的代理协议，目前 Netch 支持以下代理协议：Shadowsocks，VMess，Socks5，ShadowsocksR

与此同时 Netch 避免了 SSTap 的 NAT 问题 ，检查 NAT 类型即可知道是否有 NAT 问题。使用 SSTap 加速部分 P2P 联机，对 NAT 类型有要求的游戏时，可能会因为 NAT 类型严格遇到无法加入联机，或者其他影响游戏体验的情况

## 新手入门
[新手入门教程](Quickstart.zh-CN.md)

## 进阶用法
[进阶教程](https://github.com/NormanBB/NetchMode/blob/master/docs/README.zh-CN.md)
## 依赖（必装，否则会启动失败）
- [Visual C++ 运行库合集](https://www.google.com/search?q=Visual+C%2B%2B+%E8%BF%90%E8%A1%8C%E5%BA%93%E5%90%88%E9%9B%86)
- [.NET Framework 4.8](https://dotnet.microsoft.com/download/dotnet-framework/thank-you/net48-offline-installer)
- [TAP-Windows](https://build.openvpn.net/downloads/releases/tap-windows-9.21.2.exe)

## 语言支持
Netch 支持多种语言，在启动时会根据系统语言选择自身语言。如果需要手动切换语言，可以在启动时加入命令行参数，命令行参数为目前支持的语言代码，可以去 [NetchTranslation/i18n](https://github.com/NetchX/NetchTranslation/tree/master/i18n) 文件夹下查看外部支持的语言代码文件。Netch 目前内置 en-US，zh-CN，外置 zh-TW。欢迎大家为 [NetchTranslation](https://github.com/NetchX/NetchTranslation) 提供其他语言的翻译

## 引用
- [go-tun2socks](https://github.com/eycorsican/go-tun2socks)
- [shadowsocks-libev](https://github.com/shadowsocks/shadowsocks-libev)
- [shadowsocksr-libev](https://github.com/shadowsocksrr/shadowsocksr-libev)
- [v2ray-core](https://github.com/v2ray/v2ray-core)
- [trojan](https://github.com/trojan-gfw/trojan)
- [ACL4SSR](https://github.com/ACL4SSR/ACL4SSR)
- [dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [unbound](https://github.com/NLnetLabs/unbound)
- [tap-windows6](https://github.com/OpenVPN/tap-windows6)
- [Privoxy](https://www.privoxy.org/)
- [NatTypeTester](https://github.com/HMBSbige/NatTypeTester)
- [NetFilter SDK](https://netfiltersdk.com/)