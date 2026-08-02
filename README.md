# 推薦的好用開源iOS APP中文列表

Awesome FOSS iOS Apps list (Chinese)

一些我覺得好用的自由及開放原始碼 (Free and Open Source) 的iOS APP，適用iPhone與iPad。

**收錄標準：** 開發者需提供APP完整原始碼，並使用符合自由軟體基金會認可的自由軟體授權條款（如GPL、MPL、BSD、MIT、Apache等）。部分使用開源函式庫，但APP本體閉源發佈的不能算做開源。這些都是我用過並參考網友經驗，覺得不錯才放進列表的，有些用途太狹隘、單純只是reference implementation、沒在維護的、設計不良的APP並不會包含進去。

我了解，相較於Android能透過刷LineageOS + Degoogle + F-Droid實現近乎全開源環境，iOS不太可能做到全開源，很多日常APP都沒有替代品，要嘛只能依賴iOS內建的APP，要嘛只能使用專有軟體。這裡我盡量做到不依賴閉源軟體。尤其是綁死一個系統才能使用的軟體。希望最重要的資料可以在各大作業系統之間互通有無。

請善用右邊的目錄快速跳轉。Github可以點選README右上角的三個點顯示目錄。

註解：爲了方便讀者下載，下面收錄的APP優先以App Store的連結爲主，其次是Git原始碼儲存庫。部分APP沒有上架App Store，需要用[AltStore這類手段](https://ivonblog.com/posts/ios-sideloading/)側載。


## 第三方應用商店

| 名稱 | 簡介 |
| --- | --- |
| [AltStore](https://github.com/altstoreio/AltStore) | 用於安裝第三方IPA，APP安裝後7天內要用電腦重簽。支援啓動JIT模式。 |
| [AltStore PAL](https://altstore.io/) | 僅限歐盟地區使用的第三方商店，可以繞過App Store下載APP。|
| [SideStore](https://github.com/SideStore/SideStore) | AltStore的fork，用於安裝第三方IPA，使用線上伺服器取代電腦重簽。支援啓動JIT模式。 |
| [TrollStore](https://github.com/opa334/TrollStore) | 利用漏洞安裝任意IPA，免重簽，僅限特定iOS版本使用。支援啓動JIT模式。 |
| [Feather iOS](https://github.com/khcrysalis/Feather) | 用於安裝第三方IPA之用。支援本機簽名IPA，免用Mac電腦。建議購買Apple付費開發者憑證，即可不受7天重簽限制並安裝無限數量的IPA。 |
| [LiveContainer](https://github.com/LiveContainer/LiveContainer) | 讓APP不用安裝就能執行，藉此安裝無限數量的第三方APP。|
| [Sileo](https://github.com/Sileo/Sileo) | 越獄後通常會安裝的應用商店，替代Cydia，用於管理tweaks更新。|


## 瀏覽器

| 名稱 | 簡介 |
| --- | --- |
| [Brave Browser](https://apps.apple.com/tw/app/id1052879175) | 支援跨平臺同步。提供原生擋廣告功能，阻擋網頁追蹤器保護隱私。支援背景播放YouTube。整合Web 3的加密貨幣生態系。 |
| [Firefox](https://apps.apple.com/tw/app/id989804926) | 跨平台的開源瀏覽器，支援同步書籤和密碼。阻擋網頁追蹤器保護隱私。另外有擋廣告功能的Firefox Focus。目前使用的是WebKit引擎，尚未遷移到自研的Gecko。 |
| [Duckduckgo Browser](https://apps.apple.com/tw/app/id663592361) | 預設使用Duckduckgo作爲搜尋引擎。阻擋網頁追蹤器保護隱私。支援背景播放Youtube。 |
| [Onion Browser](https://apps.apple.com/tw/app/id519296448) | 使用Tor連線上網。 |
| [SnowHaze](https://apps.apple.com/tw/app/id1121026941) | 阻擋追蹤器與擋廣告，保護隱私。支援Tor連線。 |
| [Reynard Browser](https://github.com/minh-ton/reynard-browser) | 使用Gecko引擎的實驗性瀏覽器，不依賴WebKit。支援安裝Firefox電腦版的擴充套件。|
| [Chromium iOS](https://chromium.googlesource.com/chromium/src/+/main/ios/) |  使用Blink引擎的實驗性瀏覽器，尚未有APP採用。 |


## 網路連線

| 名稱 | 簡介 |
| --- | --- |
| [OpenVPN](https://apps.apple.com/tw/app/id590379981) | OpenVPN協定官方客戶端。 |
| [WireGuard](https://apps.apple.com/tw/app/id1441195209) | WireGuard協定官方客戶端。 |
| [IVPN](https://apps.apple.com/tw/app/id1193122683) | 直布羅陀的公司經營的VPN，需付費。 |
| [Mullvad VPN](https://apps.apple.com/tw/app/id1488466513) | 瑞典Mullvad公司經營的VPN，需付費。 |
| [ProtonVPN](https://apps.apple.com/tw/app/id1437005085) | 瑞士Proton公司經營的VPN，可用自研協定反審查，提供免費額度。 |
| [Orbot VPN iOS](https://apps.apple.com/tw/app/id1609461599) | 讓iOS全域連線走Tor上網。 |
| [Geph迷霧通](https://apps.apple.com/tw/app/id1638148282) | 翻牆工具，使用自研協定反審查，提供免費額度。 |
| [Clash Mi](https://apps.apple.com/tw/app/id6744321968) | 基於Clash.Meta的翻牆工具。 |
| [Tailscale](https://apps.apple.com/tw/app/id1470499037)  | 內網穿透VPN，基於WireGuard開發。伺服器可自架。提供MagicDNS。 |
| [NetBird](https://apps.apple.com/tw/app/id6469329339)  | 內網穿透VPN，基於WireGuard開發。伺服器可自架。 |
| [Blockada](https://apps.apple.com/tw/app/id1508341781)  | 全域擋廣告DNS，需要付費。 |
| [AdGuard](https://apps.apple.com/tw/app-bundle/id1893320718) | 全域擋廣告DNS，需要付費。 |


## 通訊軟體

| 名稱 | 簡介 |
| --- | --- |
| [Element X](https://apps.apple.com/tw/app/id1631335820) | Elements公司經營的，支援Matrix協定的點對點加密聊天APP，提供視訊通話，類似Discord。 |
| [FluffyChat](https://apps.apple.com/tw/app/id1551469600)  | 非營利組織開發的，支援Matrix協定的點對點加密聊天APP。 |
| [Mumble-iOS](https://apps.apple.com/tw/app/id443472808) | 遊戲語音群聊軟體。|
| [ProtonMail](https://apps.apple.com/tw/app/id979659905)  | 瑞士公司經營的加密電子郵件服務。 |
| [Tutanota](https://apps.apple.com/tw/app/id922429609) | 德國公司經營的加密電子郵件服務。 |
| [SimpleX](https://apps.apple.com/tw/app/id1605771084)  | 點對點加密通訊軟體，使用雙棘輪加密反竊聽，註冊不需要電子郵件或電話號碼。 |
| [Signal](https://apps.apple.com/tw/app/id874139669)  | 非營利組織經營的點對點加密通訊軟體，使用雙棘輪加密反竊聽。註冊需要電話號碼。 |
| [Telegram](https://apps.apple.com/tw/app/id686449807) | 免費通訊軟體，支援點對點加密。註冊需要電話號碼。 |
| [Thunderbird](https://github.com/thunderbird/thunderbird-ios)  | 開源電子郵件客戶端，開發中。 |


## 主題裝飾

|名稱|簡介|
|---|---|
|||


## 檔案管理器

|名稱|簡介|
|---|---|
|||


## 生產力

| 名稱 | 簡介 |
| --- | --- |
| [Simplenote](https://apps.apple.com/tw/app/id289429962) | 跨平台Markdown筆記軟體，有網頁版。可以把筆記公開成網頁。 |
| [Standard Notes](https://apps.apple.com/tw/app/id1285392450) | 跨平台Markdown筆記軟體，有網頁版。伺服器能夠自架。可以把筆記公開到Listed的網址，還能寄送電子報。 |
| [Joplin](https://apps.apple.com/tw/app/id1315599797) | 跨平台筆記兼待辦事項，類似Evernote，使用Markdown儲存筆記。支援加密雲端同步，伺服器能夠自架。提供簡易手寫筆記，還有很多擴充功能。可以把筆記公開成網頁。 |
| [Saber](https://apps.apple.com/tw/app/id1671523739) | 手寫優先的筆記工具，跨平台，支援注解PDF。可透過Nextcloud同步。 |
| [FSNotes](https://apps.apple.com/tw/app/id1346501102) | 適用iOS與macOS的筆記整理軟體，使用Markdown儲存筆記，可透過Git同步。 |
| [思源筆記 SiYuan](https://apps.apple.com/tw/app/id1583226508) |跨平台個人知識管理系統，提供Markdown和區塊式編輯，還有許多心智圖模板。伺服器能夠自架。 |
| [Logseq](https://apps.apple.com/tw/app/id1601013908) | 條列式筆記管理軟體，可以繪製筆記關聯圖，支援Markdown。|
| [Notesnook](https://apps.apple.com/tw/app/id1544027013) | 跨平臺零知識加密的筆記軟體，支援雙向筆記。 |
| [Trinote](https://apps.apple.com/tw/app/id6761228249)  | Trilium客戶端，需要連線到遠端伺服器。跨平台個人知識管理系統。 |
| [AFFiNE](https://apps.apple.com/tw/app/id6736937980) | 跨平台知識管理工具，有網頁版，提供Markdown筆記、看板管理、手寫畫布，類似Notion + Milo + Heptabase的混合體。伺服器可自架。可以把筆記公開成網頁。 |
| [AnyType](https://apps.apple.com/tw/app/id6449487029)  | 跨平台知識管理工具，可以建立筆記關聯圖。 |
| [AppFlowy](https://apps.apple.com/tw/app/id6457261352)  |跨平台知識管理工具，多人協作筆記軟體，支援看板管理。 |
| [Collabora Office](https://apps.apple.com/tw/app/collabora-office/id1440482071) | Microsoft Office替代品，LibreOffice的fork。適合開啟ODF格式的文件、試算表、投影片。 |
| [OnlyOffice](https://apps.apple.com/tw/app/id944896972)| Microsoft Office替代品，適合開啟ODF與Word的文件。 |
| [OpenDocument Reader](https://apps.apple.com/tw/app/id1510195065)  | 開啓與編輯ODF檔案。 |
| [Nextcloud](https://apps.apple.com/tw/app/id1125420102) | 自架雲端硬碟，內建Nextcloud Office網頁版功能。 |
| [Mattermost](https://apps.apple.com/tw/app/id1257222717) | 開源群組通訊系統，類似Slack。 |
| [Jami](https://apps.apple.com/tw/app/id1306951055) | 開源遠端會議應用，點對點加密，使用不需要註冊，伺服器可自架。 |
| [Jitsi Meet](https://apps.apple.com/tw/app/id1165103905) | 開源遠端會議應用，使用不需要註冊，伺服器可自架。 |
| [OpenFind](https://apps.apple.com/tw/app/id6443969902)  | 搜尋圖片中的文字。 |
| [Clip](https://github.com/rileytestut/Clip) | 剪貼簿歷史管理工具。 |
| [Foqos](https://apps.apple.com/tw/app/id6736793117) | 封鎖APP或網站，保存專注。需要掃QR Code或者NFC tag才能解鎖APP。 |


## 多媒體

| 名稱 | 簡介 |
| --- | --- |
| [VLC](https://apps.apple.com/tw/app/id650377962)  | 萬能影片播放器，支援大多數格式的影片和音樂。可以背景播放。|
| [Readest](https://apps.apple.com/tw/app/id6738622779) | 電子書閱讀器，支援EPUB、1MOBI、KF8 (AZW3)、FB2, CBZ、TXT、PDF格式，能在書本上劃記重點。可存取OPDS/Calibre伺服器。支援跨平臺同步閱讀進度，包括KOReader。 |
| [BookPlayer](https://apps.apple.com/tw/app/id1138219998) | 有聲書播放器，提供睡眠定時器功能。 |
| [MetaX](https://apps.apple.com/tw/app/id1376589355) | 編輯照片EXIF，一鍵刪除照片GPS資料。 |
| [Moblin](https://apps.apple.com/tw/app/id6466745933) | 直播軟體，串流UVC相機畫面。可搭配空拍機使用。 |
| [VDO Ninja](https://github.com/steveseguin/vdo.ninja) |讓手機鏡頭與麥克風變成電腦的Webcam，並投影到網頁串流。|


## 導航

| 名稱 | 簡介 |
| --- | --- |
| [OSMAnd](https://apps.apple.com/us/app/id934850257)  | 基於OpenStreetMap的導航APP，提供全球地圖的離線資料，支援3D地圖。|
| [Organic Maps](https://apps.apple.com/tw/app/id1567437057) | 基於OpenStreetMap的導航APP，提供全球地圖的離線資料。 |
| [OSS Weather](https://apps.apple.com/us/app/id1499117252) | 使用OpenWeather、Open-Meteo、Meteo France獲取天氣預報。 |


## 社群媒體

| 名稱 | 簡介 |
| --- | --- |
| [Bluesky](https://apps.apple.com/tw/app/id6444370199) | 去中心化社群媒體。 |
| [Mastodon](https://apps.apple.com/tw/app/id1571998974)  | 去中心化社群媒體。 |
| [Infinity for Reddit](https://apps.apple.com/tw/app/id6759064642) | 無廣告第三方Reddit客戶端。 |
| [Wordpress](https://apps.apple.com/tw/app/id335703880)  | 官方客戶端，線上存取Wordpress網站。 |
| [FeedFlow](https://apps.apple.com/tw/app/id6447210518) | RSS閱讀器。 |
| [NetNewsWire](https://apps.apple.com/tw/app/id1480640210) | RSS閱讀器，支援跨裝置同步。 |
| [JHentai](https://github.com/jiangtian616/JHenTai) | 使用Flutter寫成的跨平台E-hentai閱讀器，提供雙頁閱讀界面，可以下載漫畫離線閱讀。 |
| [EhPanda](https://github.com/EhPanda-Team/EhPanda) | 使用Swift寫成的E-hentai閱讀器，支援雙頁模式。不能下載漫畫，只能下載種子。 |
| [Aidoku](https://github.com/Aidoku/Aidoku) | 看漫畫APP，透過安裝擴充套件存取各大漫畫網站。 |
| [Mangayomi](https://github.com/kodjodevf/mangayomi) | 看漫畫與動漫的APP，模仿Mihon的設計理念，透過安裝擴充套件存取各大漫畫網站。 |
| [Paperback](https://apps.apple.com/tw/app/id1626613373) | 看漫畫APP，透過安裝擴充套件存取各大漫畫網站。 |
| [Yattee](https://github.com/yattee/yattee) | 無廣告Youtube客戶端，透過連線到yt-dlp伺服器來觀看Youtube影片，也可以存取Invidous站台代理Youtube影片。|
| [YouTube Plus](https://github.com/dayanch96/YTLite) | 針對Youtube官方APP修改的版本，加入許多自定義功能，例如懸浮播放、去廣告、顯示倒讚、SponsorBlock擋業配廣告。需要付費才能使用。|


## 健康

|名稱|簡介|
|---|---|
|||


## 理財

|名稱|簡介|
|---|---|
| [Flow](https://apps.apple.com/tw/app/flow-expense-tracker/id6477741670) | 跨平台記帳APP，可離線使用。|


## 輸入法

| 名稱 | 簡介 |
| --- | --- |
| [AI Dictation](https://apps.apple.com/tw/app/id6754910103) | 開源語音轉文字鍵盤，支援iPhone與iPad。可在支援第三方鍵盤的文字欄位聽寫；iOS 17以上可下載離線模型，也可選用雲端轉錄與整理。[原始碼](https://github.com/writingmate/aidictation)採MIT授權。 |
| [「仓」输入法](https://apps.apple.com/tw/app/id6446617683) | 跨平臺輸入法框架RIME的iOS移植版，支援拼音、注音。提供OpenCC簡轉繁。 |
| [Fcitx5-iOS](https://github.com/fcitx-contrib/fcitx5-ios) | 跨平臺的輸入法框架，支援拼音、注音。提供OpenCC簡轉繁。 |
| [萊姆輸入法LIME](https://apps.apple.com/tw/app/id6784694460) | 繁體中文爲主的輸入法，支援注音、倉頡、大易、行列、輕鬆、速成、拼音，並有許氏與倚天鍵盤排列方式。詞庫以臺灣用語爲主。提供繁簡轉換、分離式鍵盤、語音輸入。界面有許多自定義按鈕。支援實體鍵盤。 |


## 遊戲

| 名稱 | 簡介 |
| --- | --- |
| [RetroArch](https://apps.apple.com/tw/app/id6499539433) | 經典家機遊戲模擬器，支援模擬三十款以上復古遊戲主機和電腦系統，例如：MS-DOS、PC-98、Apple Macintosh、Commodore 64、SEGA Staturn、BANDAI WonderSwan、Coleco Vision、Nintendo 64、Sony Playstation等等。 |
| [PPSSPP](https://apps.apple.com/tw/app/id6496972903) | PSP遊戲模擬器，支援金手指。 |
| [Delta](https://apps.apple.com/tw/app/id1048524688) | NES與Gameboy模擬器。 |
| [SuperTuxKart](https://apps.apple.com/tw/app/id6737858957) |自由軟體吉祥物駕駛卡丁車的賽車遊戲，3D畫面品質優秀。 |
| [Luanti](https://github.com/luanti-org/luanti) | 開源方塊遊戲，類似Minecraft，可以裝Lua語言寫成的模組。iOS版尚未上架，需要自行編譯。 |
| [Multicraft](https://apps.apple.com/tw/app/id1174039276) | Luanti的fork，界面較爲友善，內含廣告。 |
| [Angel Aura Amethyst](https://github.com/AngelAuraMC/Amethyst-iOS) | Java版Minecraft啓動器。 |
| [osu!](https://github.com/ppy/osu) | 跨平台音樂節奏遊戲。官方沒有上架App Store，需要側載IPA。 |
| [Mindustry](https://apps.apple.com/tw/app/id1385258906) | 跨平台的塔防+資源蒐集遊戲。 |


## 程式開發

| 名稱 | 簡介 |
| --- | --- |
| [iSH Shell](https://apps.apple.com/tw/app/ish-shell/id1436902243) | 32位元Alpine Linux模擬器，翻譯x86指令，用終端機跑ssh、vim、yt-dlp、ffmpeg、Python之類的指令小工具。 |
| [a-Shell](https://apps.apple.com/tw/app/a-shell/id1473805438)| 終端機，功能類似iSH Shell但效能更好，因爲針對iOS原生編譯。但是無法自由安裝套件，只能用作者提供的WASM包。支援跑Python Jupyter Notebook。|
| [Blink Shell](https://apps.apple.com/tw/app/blink-shell-build-code/id1594898306) | 專業級的終端機APP，可以搭配VSCode使用。雖然開源但是App Store版本是訂閱制軟體。 |
| [NewTerm](https://github.com/hbang/NewTerm) | iOS終端機，需要越獄才能使用。|
| [Code App by thebaselab](https://apps.apple.com/tw/app/code-app/id1512938504)| 介面長得很像Visual Studio Code的IDE，內建Git與終端機，支援編譯原生Python、NodeJS、PHP、C、Java程式。App Store版為付費軟體。 |
| [Harbour](https://apps.apple.com/tw/app/id1582439659) | 遠端管理Portainer的Docker容器。 |
| [Edhita](https://apps.apple.com/tw/app/id398896655) | 文字編輯器，兼具HTML預覽功能。 |


## 實用工具

| 名稱 | 簡介 |
| --- | --- |
| [Bitwarden](https://apps.apple.com/tw/app/id1137397744) | 跨平台同步的密碼管理器。 |
| [Floccus](https://apps.apple.com/tw/app/id1626998357)| 跨平台同步瀏覽器書籤。|
| [KDE Connect](https://apps.apple.com/tw/app/id1580245991) | 跨平台傳檔案，共享剪貼簿，手機當電腦遙控器。 |
| [LocalSend](https://apps.apple.com/tw/app/id1661733229)  | 跨平台檔案分享，不用註冊帳號。 |
| [RustDesk](https://apps.apple.com/tw/app/id1581225015) | 開源免費的遠端桌面，中繼伺服器可以自架。 |
| [Moonlight Game Streaming](https://apps.apple.com/tw/app/id1000551566) | 遠端桌面兼雲端串流遊戲，支援低延遲與HDR。 |
| [AirDash](https://apps.apple.com/tw/app/id1596599922) | 跨平臺傳檔工具。|
| [OnionShare](https://apps.apple.com/tw/app/id1601890129) | 透過Tor網路匿名分享檔案。|
| [Free42](https://apps.apple.com/tw/app/id337692629) | 模擬HP-42S介面的科學工程計算機。 |
