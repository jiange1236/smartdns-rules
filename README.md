# 简介

本项目生成适用于 [**Smartdns**] 的规则集（DOMAIN-SET、IP-SET、RULE-SET 和 IP-CIDR）。使用 GitHub Actions 北京时间每天早上 6:30 自动构建，保证规则最新。

## 说明

本项目规则集（DOMAIN-SET、IP-SET、RULE-SET 和 IP-CIDR）的数据主要来源于项目 [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) 和 [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)；[`Apple`](https://github.com/jiange1236/smartdns-rules/blob/release/Loyalsoldier/apple-cn.txt) 和 [`Google`](https://github.com/jiange1236/smartdns-rules/blob/release/Loyalsoldier/google-cn.txt) 列表里的部分域名来源于项目 [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)；中国大陆 IPv4 地址数据使用 [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)。

## 规则文件地址及使用方式

### 在线地址（URL）

> 如果无法访问域名 `raw.githubusercontent.com`，可以使用第二个地址（`cdn.jsdelivr.net`），但是内容更新会有 12 小时的延迟。

#### DOMAIN-SET:

- **直连域名列表 direct-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/direct-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/direct-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/direct-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/direct-list.txt)
- **代理域名列表 proxy-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/proxy-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/proxy-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/proxy-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/proxy-list.txt)
- **广告域名列表 reject-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/reject-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/reject-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/reject-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/reject-list.txt)
- **中国大陆域名列表 china-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/china-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/china-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/china-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/china-list.txt)
- **私有网络专用域名列表 private.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/private.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/private.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/private.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/private.txt)
- **Apple 在中国大陆可直连的域名列表 apple-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/apple-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/apple-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/apple-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/apple-cn.txt)
- **iCloud 域名列表 icloud.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/icloud.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/icloud.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/icloud.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/icloud.txt)
- **[慎用]Google 在中国大陆可直连的域名列表 google-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/google-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/google-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/google-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/google-cn.txt)
- **GFWList 域名列表 gfw.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/gfw.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/gfw.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/gfw.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/gfw.txt)
- **非中国大陆使用的顶级域名列表 tld-not-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/tld-not-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/tld-not-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/tld-not-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/tld-not-cn.txt)
###### 1-stream
- **非中国大陆域名列表 stream.smartdns.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/1-stream/stream.smartdns.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/1-stream/stream.smartdns.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/1-stream/stream.smartdns.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/1-stream/stream.smartdns.txt)
###### Clang
- **中国大陆域名列表 Clang-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Clang/Clang-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Clang/Clang-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Clang/Clang-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Clang/Clang-cn.txt)
###### blackmatrix7
- **中国大陆域名列表 ChinaMax_Domain.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/blackmatrix7/ChinaMax_Domain.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/blackmatrix7/ChinaMax_Domain.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/blackmatrix7/ChinaMax_Domain.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/blackmatrix7/ChinaMax_Domain.txt)
- **非中国大陆域名列表 Global_Domain.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/blackmatrix7/Global_Domain.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/blackmatrix7/Global_Domain.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/blackmatrix7/Global_Domain.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/blackmatrix7/Global_Domain.txt)
###### felixonmars
- **中国大陆域名列表 accelerated-domains.china.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/felixonmars/accelerated-domains.china.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/felixonmars/accelerated-domains.china.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/felixonmars/accelerated-domains.china.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/felixonmars/accelerated-domains.china.txt)
- **Apple 在中国大陆可直连的域名列表 apple.china.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/felixonmars/apple.china.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/felixonmars/apple.china.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/felixonmars/apple.china.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/felixonmars/apple.china.txt)
- **Google 在中国大陆可直连的域名列表 google.china.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/felixonmars/google.china.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/felixonmars/google.china.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/felixonmars/google.china.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/felixonmars/google.china.txt)
###### gaoyifan
- **中国大陆域名列表 gaoyifan-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/gaoyifan/gaoyifan-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/gaoyifan/gaoyifan-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/gaoyifan/gaoyifan-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/gaoyifan/gaoyifan-cn.txt)

#### IP-SET:

- **中国大陆 IP 地址列表 cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cn.txt)
- **私有网络专用 IP 地址列表 private.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/private.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/private.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/private.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/private.txt)
- **Cloudflare 使用的 IP 地址列表 cloudflare.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cloudflare.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cloudflare.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cloudflare.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cloudflare.txt)
- **Cloudfront 使用的 IP 地址列表 cloudfront.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cloudfront.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cloudfront.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cloudfront.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cloudfront.txt)
- **Facebook 使用的 IP 地址列表 facebook.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/facebook.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/facebook.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/facebook.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/facebook.txt)
- **Fastly 使用的 IP 地址列表 fastly.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/fastly.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/fastly.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/fastly.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/fastly.txt)
- **Google 使用的 IP 地址列表 google.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/google.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/google.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/google.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/google.txt)
- **Netflix 使用的 IP 地址列表 netflix.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/netflix.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/netflix.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/netflix.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/netflix.txt)
- **Telegram 使用的 IP 地址列表 telegram.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/telegram.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/telegram.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/telegram.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/telegram.txt)
- **Twitter 使用的 IP 地址列表 twitter.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/twitter.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/twitter.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/twitter.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/twitter.txt)
###### IP-SET(special):
- **中国大陆 IP + 私有网络专用 IP 地址列表 cn+private.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cn+private.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipset/cn+private.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cn+private.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipset/cn+private.txt)

#### RULE-SET:

- **直连域名列表 direct-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/direct-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/direct-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/direct-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/direct-list.txt)
- **代理域名列表 proxy-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/proxy-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/proxy-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/proxy-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/proxy-list.txt)
- **广告域名列表 reject-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/reject-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/reject-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/reject-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/reject-list.txt)
- **中国大陆域名列表 china-list.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/china-list.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/china-list.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/china-list.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/china-list.txt)
- **私有网络专用域名列表 private.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/private.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/private.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/private.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/private.txt)
- **Apple 在中国大陆可直连的域名列表 apple-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/apple-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/apple-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/apple-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/apple-cn.txt)
- **iCloud 域名列表 icloud.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/icloud.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/icloud.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/icloud.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/icloud.txt)
- **[慎用] Google 在中国大陆可直连的域名列表 google-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/google-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/google-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/google-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/google-cn.txt)
- **GFWList 域名列表 gfw.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/gfw.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/gfw.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/gfw.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/gfw.txt)
- **非中国大陆使用的顶级域名列表 tld-not-cn.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/tld-not-cn.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ruleset/tld-not-cn.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/tld-not-cn.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ruleset/tld-not-cn.txt)

##### IP-CIDR:

- **中国大陆 IP 地址列表 cn-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/cn-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/cn-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/cn-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/cn-cidr.txt)
- **私有网络专用 IP 地址列表 private-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/private-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/private-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/private-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/private-cidr.txt)
- **Cloudflare 使用的 IP 地址列表 cloudflare-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/cloudflare-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/cloudflare-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/cloudflare-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/cloudflare-cidr.txt)
- **Cloudfront 使用的 IP 地址列表 cloudfront-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/cloudfront-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/cloudfront-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/cloudfront-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/cloudfront-cidr.txt)
- **Facebook 使用的 IP 地址列表 facebook-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/facebook-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/facebook-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/facebook-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/facebook-cidr.txt)
- **Fastly 使用的 IP 地址列表 fastly-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/fastly-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/fastly-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/fastly-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/fastly-cidr.txt)
- **Google 使用的 IP 地址列表 google-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/google-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/google-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/google-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/google-cidr.txt)
- **Netflix 使用的 IP 地址列表 netflix-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/netflix-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/netflix-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/netflix-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/netflix-cidr.txt)
- **Telegram 使用的 IP 地址列表 telegram-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/telegram-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/telegram-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/telegram-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/telegram-cidr.txt)
- **Twitter 使用的 IP 地址列表 twitter-cidr.txt**：
  - [https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/twitter-cidr.txt](https://raw.githubusercontent.com/jiange1236/smartdns-rules/release/Loyalsoldier/ipcidr/twitter-cidr.txt)
  - [https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/twitter-cidr.txt](https://cdn.jsdelivr.net/gh/jiange1236/smartdns-rules@release/Loyalsoldier/ipcidr/twitter-cidr.txt)

### 使用方式

关于 Smartdns 的详细使用方法，见[官方手册](https://pymumu.github.io/smartdns)。


## 致谢

- [@Loyalsoldier/surge-rules](https://github.com/Loyalsoldier/surge-rules)
- [@Loyalsoldier/geoip](https://github.com/Loyalsoldier/geoip)
- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)
- [@jklolixxs/SmartDNS_Rule](https://github.com/jklolixxs/SmartDNS_Rule)

## 项目 Star 数增长趋势

[![Stargazers over time](https://starchart.cc/jiange1236/smartdns-rules.svg)](https://starchart.cc/jiange1236/smartdns-rules)
