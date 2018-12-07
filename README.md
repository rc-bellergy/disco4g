# 用 4G/LTE 遙控 Parrot Disco (softmod)

## 這是什麼？
Disco4G 是為 Parrot Disco 提供的軟件修改 (softmod)。除了使用原裝的 Wi-Fi 遙控，它還提供了 4G/LTE 移動網絡來連結 Skycontroller 2 和 Disco。遙控和直播視頻都可以通過 4G/LTE 網絡傳送。換句話說，Disco可以飛到任何距離！唔，其實它還是受制於電池容量和 4G 訊號的。 :stuck_out_tongue_winking_eye:

[![Youtube video](https://uavpal.com/img/yt_thumbail_github.png)](https://www.youtube.com/watch?v=e9Xl3tTwReQ)
<img src="https://designquest.com.hk/share/disco4g/body.jpg" alt="Parrot Disco 4G softmod" style="width:395px;">

好處：
- 飛行距離不再受制於 WiFi 訊號
- 低成本 (改裝費小於 HK$400)
- 原裝硬件照常使用 (包括 Parrot Skycontroller 2 和 FreeFlight Pro App)
- 如訊號中斷，返航(RTH)功能自動開動
- 使用 [Glympse](https://www.glympse.com/get-glympse-app/) 提供獨立的實時 GPS 位置更新
- 以 Skycontroller 2 按鍵啓動 4G/LTE 遙控，容易使用
 
壞處：
- 受制於 [4G/LTE 移動網絡的覆蓋](https://zh.wikipedia.org/wiki/%E5%90%84%E5%9C%8B4G_LTE%E6%BB%B2%E9%80%8F%E7%8E%87%E5%88%97%E8%A1%A8) 
- 使用移動數據會有額外費用
- 比 Wi-Fi 有較大的延遲 (latency)

## 它如何運作?
![High-level connection diagram](https://designquest.com.hk/share/disco4g/disco4g-chart.jpg)

## 預備：
*硬件要求:*
- Parrot Disco
- Parrot Skycontroller 2 (如果是黑色操縱桿的 Skycontroller 2P，請看 [Beta](https://github.com/uavpal/disco4g/issues/18#issuecomment-402980602))
- [華為 E3372 4G USB modem](https://consumer.huawei.com/en/mobile-broadband/e3372/specs/) 和 SIM card\
注意： 華為 E3372 也有很多不同的版本，請看[這篇 FAQ](https://github.com/uavpal/disco4g/wiki/FAQ#e3372models) 選擇適合你的版本。（在香港可使用 E3372h)
- 4G USB modem 的天綫兩條 CRC9 接頭 [參考](https://bit.ly/2ryfSy9)
- [USB OTG 線](https://bit.ly/2EknoFb) 因為電池位置的限制，最好是轉90度的。
- Mobile device/phone with Wi-Fi tethering and SIM card (for best performance, use the same operator as the USB modem's SIM card)
- PC with Wi-Fi (one-time, required for initial installation)

*Software:*
- FreeFlight Pro App on tablet/phone (can be the same device providing Wi-Fi tethering)
- Zerotier account (free)
- Glympse App for independent real-time GPS tracking (optional) - free Glympse Developer account required

*<a name="supportedhw">Successfully tested using:</a>*
- Mobile tethering device: iPhone X (iOS 11.3+)
- 4G/LTE USB Modem: Huawei E3372s-153, E3372h-153, E3372h-510, E3372h-607
- USB-connected device with FreeFlight Pro App: iOS 11 - 12, most Android devices
- Parrot Disco, Firmware 1.4.1, 1.7.0, 1.7.1
- Parrot Skycontroller 2, Firmware 1.0.7 to 1.0.9
- FreeFlight Pro 5.2.0 - 5.2.2 on iOS and Android

[Drop us a note](https://github.com/uavpal/disco4g/#contactcontribute) if you have successfully tested different configurations, so we can keep this list updated.

## Installation
Please see Wiki article [Installation](https://github.com/uavpal/disco4g/wiki/Installation).

## How to fly on 4G/LTE? (User Manual)
Please see Wiki article [How to fly on 4G/LTE? (User Manual)](https://github.com/uavpal/disco4g/wiki/How-to-fly-on-4G-LTE-(User-Manual)).

## FAQ
Please see Wiki article [FAQ](https://github.com/uavpal/disco4g/wiki/FAQ).

## Is it really free? Are you crazy?
Yes and yes! This softmod has been developed over countless of days and nights by RC hobbyists and technology enthusiasts with zero commercial intention.
Anyone can download our code for free and transform his/her Disco into a 4G/LTE enabled fixed-wing drone by following the instructions provided.

_However_, we highly appreciate [feedback and active contribution](#contactcontribute) to improve and maintain this project.

![Shut up and take my money!](http://image.ibb.co/cLw9SS/shut_up_and_take_my_money.jpg)

If you insist, feel free to donate any amount you like. We will mainly use donations to acquire new hardware to be able to support a wider range of options (such as more 4G/LTE USB Modems).

[![Donate using Paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=GY3BTZPLPBB2W&lc=US&item_name=UAVPAL&cn=Add%20special%20instructions%3A&no_shipping=1&currency_code=USD&bn=PP-DonationsBF:btn_donateCC_LG.gif:NonHosted)

## Contact/Contribute
Join our [UAVPAL Slack workspace](https://join.slack.com/t/uavpal/shared_invite/enQtMzQ4NDA5NzU0MDM5LTcyNjVjMjdkMDU4ODYwYjJmZjg1MWJmMWQwYzQyOTYzZDJiNTYwNzY3MzFiMjQ1NmIwYWE2YjQ0NzdkYWFiMGQ) or check out the [issue section](https://github.com/uavpal/disco4g/issues) here on GitHub.\
Email: <img valign="bottom" src="https://image.ibb.co/mK4krx/uavpalmail2.png"> (please do not use email for issues/troubleshooting help. Join our Slack community instead!)

## Special Thanks to
- Parrot - for building this beautiful bird, as well as for promoting and supporting Free and Open-Source Software
- ZeroTier - awesome product and excellent support
- Glympse - great app and outstanding API
- Andres Toomsalu
- AussieGus
- Brian
- Carlo Comin
- [Dustin Dunnill](https://www.youtube.com/channel/UCVQWy-DTLpRqnuA17WZkjRQ)
- John Dreadwing
- [Joris Dirks](https://djoris.nl)
- Josh Mason
- Phil
- Tim Vu

## Disclaimer
This is still an EXPERIMENTAL modification, no thorough testing has been conducted! Mod and fly your Disco at YOUR OWN RISK!!!


