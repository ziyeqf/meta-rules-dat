**下载地址**：

- **country.mmdb**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/country.mmdb)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/country.mmdb)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/country.mmdb)
  
- **geoip.dat**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geoip.dat)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geoip.dat)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geoip.dat)

- **geoip.db**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geoip.db)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geoip.db)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geoip.db)

- **cn.mmdb**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/cn.mmdb)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn.mmdb)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn.mmdb)
  
- **cn.dat**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/cn.dat)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn.dat)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn.dat)

- **cn.db**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/cn.db)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn.db)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn.db)
  
- **geosite.dat**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geosite.dat)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geosite.dat)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geosite.dat)

- **geosite.db**
  - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/geosite.db)
  - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geosite.db)
  - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/geosite.db)
  
- **rule-set**
  - **cn_domain.yaml**
    - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/cn_domain.yaml)
    - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn_domain.yaml)
    - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn_domain.yaml)
    
  - **proxy.yaml**
    - [Github release](https://github.com/MetaCubeX/meta-rules-dat/releases/download/latest/proxy.yaml)
    - [JSdelivr](https://cdn.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/proxy.yaml)
    - [JSdelivr-CF](https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/proxy.yaml)
### country.mmdb,geoip.dat,geoip.db

同 [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)
- 新增类别（方便有特殊需求的用户使用）：
  - `geoip:cloudflare`
  - `geoip:cloudfront`
  - `geoip:facebook`
  - `geoip:fastly`
  - `geoip:google`
  - `geoip:netflix`
  - `geoip:telegram`
  - `geoip:twitter`

### country.mmdb,geoip.dat,geoip.db

国家仅包含CN,精简体积,替换一些类别
- 新增类别（方便有特殊需求的用户使用）：
  - `geoip:cloudflare`
  - `geoip:cloudfront`
  - `geoip:facebook`
  - `geoip:bilibili`
  - `geoip:google`
  - `geoip:netflix`
  - `geoip:telegram`
  - `geoip:twitter`

### geosite.dat,geosite.db

用法同 [Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)  
  - `geosite:cn` 源替换为 [ios_rule_script/ChinaMax_Domain](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash/ChinaMax)
  - `geosite:onedrive` 合并 [ios_rule_script/OneDrive](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash/OneDrive)
  - `geosite:steam@cn` 合并 [ios_rule_script/SteamCN](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash/SteamCN) 的内数据
  - 新增类别
    - `geosite:biliintl` 来源 [biliintl](https://raw.githubusercontent.com/xishang0128/rules/main/biliintl.list)
    - `geosite:tracker` 来源 [TrackersList](https://trackerslist.com/#/zh)以及[blackmatrix7
/
ios_rule_script](https://github.com/blackmatrix7/ios_rule_script/tree/master/rule/Clash/PrivateTracker)

### 示例
```yaml
rule-providers:
  cn:
    behavior: domain
    interval: 86400
    path: ./provider/rule-set/cn_domain.yaml
    type: http
    url: "https://testingcf.jsdelivr.net/gh/MetaCubeX/meta-rules-dat@release/cn_domain.yaml"

rules:
  - RULE-SET,cn,DIRECT
  - GEOSITE,category-ads-all,REJECT
  - GEOSITE,private,DIRECT
  - GEOSITE,youtube,PROXY
  - GEOSITE,google,PROXY
  - GEOSITE,twitter,PROXY
  - GEOSITE,pixiv,PROXY
  - GEOSITE,category-scholar-!cn,PROXY
  - GEOSITE,biliintl,PROXY
  - GEOSITE,onedrive,DIRECT
  - GEOSITE,microsoft@cn,DIRECT
  - GEOSITE,apple-cn,DIRECT
  - GEOSITE,steam@cn,DIRECT
  - GEOSITE,category-games@cn,DIRECT
  - GEOSITE,geolocation-!cn,PROXY
  - GEOSITE,cn,DIRECT
  
  #GEOIP规则
  - GEOIP,private,DIRECT,no-resolve
  - GEOIP,telegram,PROXY
  - GEOIP,JP,PROXY
  - GEOIP,CN,DIRECT
  - DST-PORT,80/8080/443/8443,PROXY
  - MATCH,DIRECT
```

## 致谢

- [@Loyalsoldier/geoip](https://github.com/Loyalsoldier/geoip)
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)
- [@Loyalsoldier/domain-list-custom](https://github.com/Loyalsoldier/domain-list-custom)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@gfwlist/gfwlist](https://github.com/gfwlist/gfwlist)
- [@cokebar/gfwlist2dnsmasq](https://github.com/cokebar/gfwlist2dnsmasq)
- [@Loyalsoldier/cn-blocked-domain](https://github.com/Loyalsoldier/cn-blocked-domain)
- [@AdblockPlus/EasylistChina+Easylist.txt](https://easylist-downloads.adblockplus.org/easylistchina+easylist.txt)
- [@AdGuard/DNS-filter](https://kb.adguard.com/en/general/adguard-ad-filters#dns-filter)
- [@PeterLowe/adservers](https://pgl.yoyo.org/adservers)
- [@DanPollock/hosts](https://someonewhocares.org/hosts)
- [@crazy-max/WindowsSpyBlocker](https://github.com/crazy-max/WindowsSpyBlocker)
- [@blackmatrix7/ios_rule_script](https://github.com/blackmatrix7/ios_rule_script)
