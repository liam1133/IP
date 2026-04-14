# IPDB API

![Version](https://img.shields.io/badge/version-2.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Status](https://img.shields.io/badge/status-active-brightgreen.svg)

**高性能 IP 地址信息获取服务**

`https://ipdb.api.030101.xyz`

---

**联系方式**

[![Telegram](https://img.shields.io/badge/群聊-HeroCore-blue?logo=telegram&logoColor=white)](https://t.me/HeroCore) 
[![Telegram](https://img.shields.io/badge/频道-HeroMsg-blue?logo=telegram&logoColor=white)](https://t.me/HeroMsg)

**DO NOT UPDATE**



Cloudflare大善人的Workers可以搭建节点，大佬们靠爱发电更新的proxyip一直不稳定，导制很多cloudflare网站打不开。今天闲下来了配置一个自动抓取proxyip然后DDNS更新。

github创建一个项目，在项目根目录创建 .github/workflows/update-proxy-ip.yml

在GitHub仓库的Settings → Secrets中添加：

CLOUDFLARE_ZONE_ID：应该是类似 a1b2c3d4e5f6g7h8i9j0 的字符串

CLOUDFLARE_API_TOKEN：以 Bearer 开头的API令牌

DOMAIN_NAME：完整的域名，如 proxy.example.com

手动运行一次，看ip有没有保存到仓库。

运行完成无报错，看DDNS更新没有。更新了即成功！
