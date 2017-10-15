Here's the page answering questions: does A support B?

## Servers

                  | [Python]  |   [libev]   |    [Go]   
----------------- | --------- | ----------- | ----------
Fast Open         |     Y     |      Y      |      N  
Multiple Users    |     Y     |      Y      |      Y   
Management API    |     Y     |      Y      |      N   
Workers           |     Y     |      N      |      N   
Graceful Restart  |     Y     |      N      |      N   
ss-redir          |     N     |      Y      |      N   
ss-tunnel         |     N     |      Y      |      N   
UDP Relay         |     Y     |      Y      |      N
OTA               |     Y     |      Y      |      Y   

## Clients

                   | [Windows] | [ShadowsocksX] | [Qt5] | [Android] | [iOS App Store] | [iOS Cydia]
------------------ | --------- | -------------- | ----- | ------- | ------------- | ---------
System Proxy       |    Y      |      Y         |  N    |    Y    |        N      |     Y
CHNRoutes          |    Y      |      Y         |  N    |    Y    |        Y      |     Y
PAC Configuration  |    Y      |      Y         |  N    |    N    |        N      |     N
Profile Switching  |    Y      |      Y         |  Y    |    Y    |        N      |     Y
QR Code Scan       |    Y      |      Y         |  Y    |    Y    |        Y      |     Y
QR Code Generation |    Y      |      Y         |  Y    |    Y    |        N      |     Y

[Python]: https://github.com/shadowsocks/shadowsocks
[libev]: https://github.com/shadowsocks/shadowsocks-libev
[Go]: https://github.com/shadowsocks/shadowsocks-go
[node.js]: https://github.com/shadowsocks/shadowsocks-nodejs
[Windows]: https://github.com/shadowsocks/shadowsocks-csharp
[ShadowsocksX]: https://github.com/shadowsocks/shadowsocks-iOS
[qt5]: https://github.com/shadowsocks/shadowsocks-qt5
[Android]: https://github.com/shadowsocks/shadowsocks-android
[iOS App Store]: https://github.com/shadowsocks/shadowsocks-iOS
[iOS Cydia]: https://github.com/linusyang/MobileShadowSocks