# 二级代理抓包效果

如此，即可实现，在Mac中Reqable中，抓包安卓设备中的网络请求了 == 二级代理后的抓包效果：

效果：安卓端打开Youtube：

![android_browser_youtube](../../assets/img/android_browser_youtube.png)

然后Mac端Reqable中可以抓包到流量：

![mac_reqable_see_flow](../../assets/img/mac_reqable_see_flow.png)

以及：安卓端打开Google Play商店，并尝试登录：

![android_google_play_login](../../assets/img/android_google_play_login.png)

Mac中Reqable可以抓到包：

![mac_reqable_see_google_play_1](../../assets/img/mac_reqable_see_google_play_1.png)

![mac_reqable_see_google_play_2](../../assets/img/mac_reqable_see_google_play_2.png)

另外，尝试去打开：Telegram：

![android_open_telegram](../../assets/img/android_open_telegram.png)

然后可以触发到=Reqable抓包到，相关请求：

* https://android.apis.google.com/c2dm/register3

![mac_reqable_google_api_register3_1](../../assets/img/mac_reqable_google_api_register3_1.png)

![mac_reqable_google_api_register3_2](../../assets/img/mac_reqable_google_api_register3_2.png)

