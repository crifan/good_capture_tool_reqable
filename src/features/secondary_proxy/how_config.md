# 如何配置二级代理

概述：

* Mac + Android
  * Android端：WiFi代理，设置为：Mac端Reqable的代理==协同抓包
    * 此处是：`192.168.2.14:9000`
  * Mac端：本地有能翻墙的代理，加上二级代理，且启用后，即可继续用Reqable去正常抓包
    * 且为了支持安卓端的app（Youtube、Google Play商店等）的翻墙访问外网的需求，需要给Mac端Reqable去加上二级代理
      * 二级代理用Mac端的Trojan的代理：`允许局域网访问` + `HTTP代理`是：（Trojan-QT的）`127.0.0.1:58591`

详解：

## Android端

安卓端的WiFi代理：

![android_wifi_proxy](../../assets/img/android_wifi_proxy.png)

注：安卓端的WiFi的IP地址是：`192.168.2.53`

![android_wifi_ip_1](../../assets/img/android_wifi_ip_1.png)

![android_wifi_ip_2](../../assets/img/android_wifi_ip_2.png)

## Mac端

对应着：Mac端的Reqable的代理设置

![mac_reqable_same_wifi](../../assets/img/mac_reqable_same_wifi.png)

Mac端的Trojan的代理：开启局域网共享 + HTTP代理是：127.0.0.1:58591

![mac_trojan_enable_share](../../assets/img/mac_trojan_enable_share.png)

Mac端Reqable中添加和开启：二级代理

![mac_reqable_sencond_proxy](../../assets/img/mac_reqable_sencond_proxy.png)

![reqable_sencond_proxy_config](../../assets/img/reqable_sencond_proxy_config.png)
