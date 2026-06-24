# clash pro rules简介


规则转自：Loyalsoldier，在此基础上添加Google,youtube,netflix,telegram,apple,icloud

本项目生成适用于 clash mimoho 的规则集（RULE-SET）。

## 说明

本项目的规则集（RULE-SET）开始使用AI工具搜集，不保证全面，请自行补充。部分源于项目 [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) 和 [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)；[`Apple`](https://github.com/Loyalsoldier/clash-rules/blob/release/apple.txt) 和 [`Google`](https://github.com/Loyalsoldier/clash-rules/blob/release/google.txt) 列表里的部分域名来源于项目 [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)；中国大陆 IPv4 地址数据使用 [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)。

本项目的规则集（RULE-SET）只适用于**Clash** 。支持 **TUN 增强模式**，能接管设备所有 TCP 和 UDP 流量，也支持 [mimoho](https://github.com/metacubex/mihomo) 。更多高级特性请看[官方 wiki](https://wiki.metacubex.one/)。


## 规则文件地址及使用方式

### 在线地址（URL）

### 无法访问 `raw.githubusercontent.com`的解决方法

- 方法一，修改系统hosts文件，添加`151.101.108.133 raw.githubusercontent.com` (备注，这是我的IP查询出来的，请自行按照自己网络查询) \
  查询解析的IP地址：`https://ipaddress.com/website/raw.githubusercontent.com`  
- 方法二，如果`raw.githubusercontent.com`无法链接，请使用备选链接`cdn.jsdelivr.net` 
- 方法三，选择`GitHub520`项目，请使用下载hosts文件`https://cdn.jsdelivr.net/gh/521xueweihan/GitHub520@main/hosts` 

### cdn.jsdelivr.net 无法刷新缓存解决方法
- 将 cdn.jsdelivr.net中的cdn改为 purge
- git bash中执行 \
 `curl https://purge.jsdelivr.net/gh/username/reponame@latest/file.*** `
- 浏览器直接访问 \
` https://purge.jsdelivr.net/gh/snapei/clash-pro-rules@release/xxx.txt `


> 以下地址填写在 Clash 配置文件里的 `rule-providers` 里的 `url` 配置项中。

- **Apple域名列表 apple.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/apple.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/apple.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/apple.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/apple.txt)
- **applecn域名列表 applecn.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/applecn.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/applecn.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/applecn.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/applecn.txt)
- **Google 域名列表 google.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/google.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/google.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/google.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/google.txt)
- **YOUTUBE 域名列表 youtube.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/youtube.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/youtube.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/youtube.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/youtube.txt)
- **NETFLIX 域名列表 netflix.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflix.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflix.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflix.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflix.txt)
- **NETFLIX IP 地址列表 netflixcidr.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflixcidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflixcidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflixcidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflixcidr.txt)
- **中国大陆 IPv4 地址列表 cncidr.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/cncidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/cncidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/cncidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/cncidr.txt)
- **非中国大陆使用的顶级域名列表 tld-not-cn.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tld-not-cn.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tld-not-cn.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tld-not-cn.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tld-not-cn.txt)
- **TELEGRAM 域名列表 telegram.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegram.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegram.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/telegram.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/telegram.txt)
- **Telegram 使用的 IP 地址列表 telegramcidr.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegramcidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegramcidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/telegramcidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/telegramcidr.txt)
- **TIKTOK 域名列表 tiktok.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tiktok.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tiktok.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tiktok.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tiktok.txt)
- **AI 域名列表 ai.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/ai.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/ai.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/ai.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/ai.txt)
- **ANDROID 域名列表 android.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/android.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/android.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/android.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/android.txt)
- **META 域名列表 meta.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/meta.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/meta.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/meta.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/meta.txt)
- **META 使用的 IP 地址列表 metacidr.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/metacidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/metacidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/metacidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/metacidr.txt)
- **AMAZON 域名列表 amazon.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/amazon.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/amazon.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/amazon.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/amazon.txt)
- **MICROSOFT 域名列表 microsoft.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/microsoft.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/microsoft.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/microsoft.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/microsoft.txt)
- **GITHUB 域名列表 github.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/github.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/github.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/github.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/github.txt)
- **X 域名列表 x.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/x.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/x.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/x.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/x.txt)
- **SOCIALS 域名列表 socials.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/socials.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/socials.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/socials.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/socials.txt)
- **WORKSPACE 域名列表 workspace.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/workspace.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/workspace.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/workspace.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/workspace.txt)
- **MULTIMEDIA 域名列表 multimedia.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/multimedia.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/multimedia.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/multimedia.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/multimedia.txt)
- **PROXY 域名列表 proxy.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/proxy.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/proxy.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/proxy.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/proxy.txt)

### 使用方式

关于 Clash mihomo 使用方式，请查看[mihomo](https://wiki.metacubex.one/config/) 或 [Lancellc's GitBook](https://lancellc.gitbook.io/clash/)。

#### Proxy-Groups 配置方式,自定义开关

```yaml
proxy-groups:

# GOOGLE
- name: "GOOGLE"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"

# YOUTUBE
- name: "YOUTUBE"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"

- name: "AI"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"

- name: "SOCIALS"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"

- name: "WORKSPACE"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"

- name: "MULTIMEDIA"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"

- name: "PROXY"
  type: select
  proxies:
    - "CN-HK"
    - "JP-OSAKA"
    - "US-OG"
    - "US-LA"
    - "US-ST"
    - "SG-T"
```


要想使用本项目的规则集，只需要在 Clash 配置文件中添加如下 `rule-providers` 和 `rules`。

#### Rule Providers 配置方式

```yaml
rule-providers:
  apple:
     type: http
     behavior: domain
     url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/apple.txt"
     path: ./ruleset/apple.yaml
     interval: 86400

  applecn:
     type: http
     behavior: domain
     url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/applecn.txt"
     path: ./ruleset/applecn.yaml
     interval: 86400

  google:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/google.txt"
    path: ./ruleset/google.yaml
    interval: 86400

  youtube:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/youtube.txt"
    path: ./ruleset/youtube.yaml
    interval: 86400

  netflix:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflix.txt"
    path: ./ruleset/netflix.yaml
    interval: 86400

  netflixcidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflixcidr.txt"
    path: ./ruleset/netflixcidr.yaml
    interval: 86400

  tld-not-cn:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tld-not-cn.txt"
    path: ./ruleset/tld-not-cn.yaml
    interval: 86400

  telegram:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegram.txt"
    path: ./ruleset/telegram.yaml
    interval: 86400

  telegramcidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegramcidr.txt"
    path: ./ruleset/telegramcidr.yaml
    interval: 86400

  tiktok:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tiktok.txt"
    path: ./ruleset/tiktok.yaml
    interval: 86400

  ai:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/ai.txt"
    path: ./ruleset/ai.yaml
    interval: 86400

  android:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/android.txt"
    path: ./ruleset/android.yaml
    interval: 86400    

  meta:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/meta.txt"
    path: ./ruleset/meta.yaml
    interval: 86400

  metacidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/metacidr.txt"
    path: ./ruleset/metacidr.yaml
    interval: 86400

  amazon:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/amazon.txt"
    path: ./ruleset/amazon.yaml
    interval: 86400

  microsoft:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/microsoft.txt"
    path: ./ruleset/microsoft.yaml
    interval: 86400

  github:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/github.txt"
    path: ./ruleset/github.yaml
    interval: 86400

  x:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/x.txt"
    path: ./ruleset/x.yaml
    interval: 86400

  socials:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/socials.txt"
    path: ./ruleset/socials.yaml
    interval: 86400

  workspace:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/workspace.txt"
    path: ./ruleset/workspace.yaml
    interval: 86400

  multimedia:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/multimedia.txt"
    path: ./ruleset/multimedia.yaml
    interval: 86400

  proxy:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/proxy.txt"
    path: ./ruleset/proxy.yaml
    interval: 86400


```

#### Rules 配置方式

- 以下配置中的 `PROCESS-NAME` 规则类型**只能**在 **ClashX Pro** 中使用，其余版本均不能使用，需要手动删除。
- 如果希望使用 DNS 来解析未命中域名类型规则的域名，而不是直接走代理，请删除 `cncidr` 行尾的 `,no-resolve`。
- 以下配置中，除了 `DIRECT` 和 `REJECT` 是默认存在于 Clash 中的 policy（路由策略/流量处理策略），其余均为自定义 policy，对应配置文件中 `proxies` 或 `proxy-groups` 中的 `name`。如你直接使用下面的 `rules` 规则，则需要在 `proxies` 或 `proxy-groups` 中手动配置一个 `name` 为 `PROXY` 的 policy。
- 如你希望 Apple、iCloud 和 Google 列表中的域名使用代理，则把 policy 由 `DIRECT` 改为 `PROXY`，以此类推，举一反三。

```yaml
rules:
  - PROCESS-NAME,v2ray,DIRECT
  - PROCESS-NAME,Surge%203,DIRECT
  - PROCESS-NAME,ss-local,DIRECT
  - PROCESS-NAME,privoxy,DIRECT
  - PROCESS-NAME,trojan,DIRECT
  - PROCESS-NAME,trojan-go,DIRECT
  - PROCESS-NAME,naive,DIRECT
  - PROCESS-NAME,Thunder,DIRECT
  - PROCESS-NAME,DownloadService,DIRECT
  - PROCESS-NAME,qBittorrent,DIRECT
  - PROCESS-NAME,Transmission,DIRECT
  - PROCESS-NAME,fdm,DIRECT
  - PROCESS-NAME,aria2c,DIRECT
  - PROCESS-NAME,Folx,DIRECT
  - PROCESS-NAME,NetTransport,DIRECT
  - PROCESS-NAME,uTorrent,DIRECT
  - PROCESS-NAME,WebTorrent,DIRECT
  - RULE-SET,lancidr,DIRECT,no-resolve
  - RULE-SET,cncidr,DIRECT,no-resolve
  - RULE-SET,reject,REJECT
  - RULE-SET,icloud,DIRECT
  - RULE-SET,apple,DIRECT
  - RULE-SET,google,GOOGLE
  - RULE-SET,youtube,YOUTUBE
  - RULE-SET,netflix,NETFLIX
  - RULE-SET,netflixcidr,NETFLIX,no-resolve
  - RULE-SET,gfw,PROXY
  - RULE-SET,greatfire,PROXY
  - RULE-SET,tld-not-cn,PROXY
  - RULE-SET,telegramcidr,PROXY,no-resolve
  - RULE-SET,tiktok,PROXY
  - RULE-SET,proxy,PROXY
  - RULE-SET,direct,DIRECT
  - GEOIP,CN,DIRECT
  - MATCH,PROXY
```

## 致谢

- [@Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)
- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)
