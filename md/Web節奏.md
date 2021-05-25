COMET 長輪尋

WAF   防火牆/繞過


WEB 安全
Encoding（編碼攻擊）：將指令重新編碼，來躲避網站的安全檢查或使網站程式發生錯誤。
Header Tampering（標頭竄改）：修改請求標頭，以躲過安全機制的檢查。
Path Traversal（路徑挖掘）：猜測網站路徑，以進入網站根目錄之外的資料夾或檔案。
SQL Injection（SQL隱碼注入）：目前最出名也最有殺傷力的攻擊手段之一。利用SQL程式指令迴避安全檢查，竊取管理權限，可對整個網站進行毀滅性的破壞。（筆者以前架設的小論壇就曾經被這麼踩平過……）
Cross site Scripting（跨網站指令碼攻擊）：也可寫作XSS攻擊，同樣是目前常見且有力的攻擊手法之一。它的攻擊方式有點類似釣魚網站，可將使用者導向惡意網站或假網站，然後再進行後續攻擊（如騙取密碼或植入木馬等等）。
Remote Command Execution（執行遠端命令）：基本上就是透過web介面使網站程式執行遠端指令，不過這種攻擊多半要搭配網站程式漏洞執行。
Probes（探針）：你可以把「探針」想像成一種能夠搜索漏洞的小程式。攻擊者通常會把「探針」放在一些已經被入侵的熱門網站上，當你瀏覽這些網站時，探針就會被下載下來，並開始搜索你電腦中的安全漏洞，然後通知攻擊者發動攻擊。
Known Worms（已知蠕蟲）：這個應該不用多解釋了，就是電腦蠕蟲囉，通常它們不會破壞系統本身，但卻會對網路發動攻擊，像是執行垃圾代碼，讓Web程式無法回應（這招就是底下的Denial of service）；或是大量傳送無意義訊息，吃掉網路頻寬等等。
Compromised Servers（被盜用的伺服器）：應該可以說是「管理不良的伺服器」吧。舉例來說，有些管理者在架好資料庫和網站之後，沒有修改預設的密碼，因此攻擊者可以輕鬆取得所有權限，這種伺服器就算是Compromised Servers。
Spammer Bots（垃圾回應機器人）：這也是目前很常見又很令人頭痛的攻擊之一，不過它比較像是間接傷害就是了。
Bad User Agents（不良的使用者代理）：User Agents可以翻成使用者代理，不過這跟最近要上的電影《獵殺代理人》沒啥關係，它是指一些行徑惡劣的蜘蛛（Spiders）、機器人（Robots）、爬行者（Crawler）、瀏覽器（Browser）或下載工具等等，它們可能會佔用過量的頻寬或竊取一些不應該公開的資料之類的（這麼說來迅雷跟FOXY好像都可以歸在這一類？）。
Denial of Service（阻斷服務攻擊）：雖然字母一樣，但這跟DOS沒關係，這種攻擊手法是對主機傳送大量或特殊的網路封包，使主機陷入癱瘓或耗盡資源無法運作。它的「進階版」就是惡名昭彰的「DDoS」——分散式阻斷服務攻擊，由多個地方同時發動DoS攻擊，因此主機無法利用封鎖網段等方式來防堵。
Session Hijacking（會話劫持）：這招有點算是冒用別人身份。一般來說，SessionID會被當成Cookie存到用戶端電腦，攻擊者利用這個特性，竊取電腦裡的SessionID，冒充成使用者進入網站，然後就可以竊取網站中的使用者資料（如信用卡卡號）並進行後續破壞。
Cookie Tampering（竄改Cookie）：Cookie基本上可以看成是網站上的使用者紀錄，通常甚至會包含使用者帳號、密碼等資料，這種手法可以看成是在網路上攔截Cookie封包，然後拿這個封包去欺騙伺服器，於是就可以偽裝成受害者，登入網站。


RFC 標準=>
    中文版 https://docs.huihoo.com/rfc/

文件傳輸技術
    https://cloud.tencent.com/developer/article/1532107

WebSocket=>
    https://zh.wikipedia.org/wiki/WebSocket
    
    autobahn-python - WebSocket & WAMP for Python on Twisted and asyncio.
    channels - Developer-friendly asynchrony for Django.
    websockets - A library for building WebSocket servers and clients with a focus on correctness and simplicity.


Socket，Websocket，Socket.io的差異
https://leesonhsu.blogspot.com/2018/07/socketwebsocketsocketio.html

HTTP文黨==>
    https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview
HTTP==>
    httplib