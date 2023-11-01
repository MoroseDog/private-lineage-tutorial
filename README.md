## 前言

在2019年末月，發生「嚴重特殊傳染性肺炎疫情」，是一次由嚴重急性呼吸道症候群冠狀病毒2型（SARS-CoV-2）導致的嚴重特殊傳染性肺炎（COVID-19）所引發的全球大流行疫情。隨後在2020年初迅速擴散至全球多國，逐漸變成一場全球性大瘟疫。

導致現在多數國家國民們因為防疫，人人在家無法出門，這時候因受疫情影響而火紅的部分就是線上的購物、<font size="4"><font color="red">**遊戲**</font>、會議服務…等等。

之前也有提到，在分析過部落格中的熱門文章後，決定要嘗試一些讓人感興趣的技術文件、教學；
當然一些技術文章也會持續的撰寫分享用於增進自己的經驗與技術。

這邊就不在廢話，這邊決定要初步嘗試寫關於「天堂私服」的相關技術文章，在開始之前不免俗要…

免責聲明：

- 本部落格文章中皆<font size="4"><font color="red"><u>**不提供**</u></font>任何所謂的遊戲「主程式」、「模擬器」、「登入器」…等等相關程式的下載點。
- 本部落格文章中所見之遊戲主程式和服務器端程序均來自網路發佈，<font size="4"><font color="red"><u>版本歸**原作者**</u>所有</font>。
- 本部落格文章為研究SQL資料庫與修改JAVA語法使用，<font size="4"><font color="red">並<u>**非商業用途**</u>，亦<u>**無做營運事實等任何一切商業行為**</u>。</font>
- 本部落格文章內容是為研究學習設計思想和原理為目的，<font size="4"><font color="red"><u>**絕沒有故意侵權或惡意抄襲、篡改其他遊戲內容**</u></font>！

------------------------------------------------------------------------------------------------------------------------

這邊的教學主要在於讓初出茅廬有興趣的人來看看，透過簡單說明舉例讓其了解，對於詳細深入的部分就不會在這邊提到。
如果有針對某一些技術或是關鍵字有其興趣，建議可以多使用搜尋引擎針對其關鍵字，找尋相關文章來做深入研究。

## 教學章結

- <font size="4"><font color="green">**初出茅廬**</font>
  - [Server、Client 是什麼？](https://morosedog.gitlab.io/private-lineage-20210713-private-lineage-1)
  - [Java 是什麼？](https://morosedog.gitlab.io/private-lineage-20210714-private-lineage-2)
  - [VirtualBox Windows 7 安裝](https://morosedog.gitlab.io/private-lineage-20210715-private-lineage-3)
  - [Java 的安裝](https://morosedog.gitlab.io/private-lineage-20210716-private-lineage-4)
  - [Java 的版本切換](https://morosedog.gitlab.io/private-lineage-20210717-private-lineage-5)
  - [資料庫 Database(DB) 是什麼？](https://morosedog.gitlab.io/private-lineage-20210718-private-lineage-6)
  - [資料庫 MySQL 5.6.25 的安裝](https://morosedog.gitlab.io/private-lineage-20210719-private-lineage-7)
  - [資料庫 開發管理系統 的安裝](https://morosedog.gitlab.io/private-lineage-20210720-private-lineage-8)
  - [匯入模擬器的資料庫](https://morosedog.gitlab.io/private-lineage-20210721-private-lineage-9)
  - [設定檔說明設定與啟動模擬器](https://morosedog.gitlab.io/private-lineage-20210722-private-lineage-10)
  - [主程式安裝及登入器設定與登入](https://morosedog.gitlab.io/private-lineage-20210723-private-lineage-11)
- <font size="4"><font color="#0C81A2">**連線相關**</font>
  - [IP 位址 (IP Address)](https://morosedog.gitlab.io/private-lineage-20210724-private-lineage-12)
  - [內部、外部網路](https://morosedog.gitlab.io/private-lineage-20210725-private-lineage-13)
  - [防火牆輸入輸出規則](https://morosedog.gitlab.io/private-lineage-20210726-private-lineage-14)
  - [虛擬服務器和通訊埠轉發](https://morosedog.gitlab.io/private-lineage-20210727-private-lineage-15)
  - [對外設定(撥接上網)](https://morosedog.gitlab.io/private-lineage-20210728-private-lineage-16)
  - [對外設定(數據機DHCP)](https://morosedog.gitlab.io/private-lineage-20210729-private-lineage-17)
  - [對外設定(WiFi-DHCP)](https://morosedog.gitlab.io/private-lineage-20210730-private-lineage-18)
  - <s>[對外設定(數據機 & WiFi-DHCP)](https://morosedog.gitlab.io/private-lineage-20210731-private-lineage-19)</s><font size="1"><此篇暫時沒有教學></font>
- <font size="4"><font color="#0C81A2">**登入器相關**</font>
  - [登入器簡介](https://morosedog.gitlab.io/private-lineage-20210801-private-lineage-20)
  - [登入器功能說明](https://morosedog.gitlab.io/private-lineage-20210802-private-lineage-21)
  - [登入器設定檔說明](https://morosedog.gitlab.io/private-lineage-20210803-private-lineage-22)
  - [FTP 伺服器架設(FileZilla)](https://morosedog.gitlab.io/private-lineage-20210804-private-lineage-23)
  - [登入器自動更新伺服器列表](https://morosedog.gitlab.io/private-lineage-20210805-private-lineage-24)
  - [登入器自動更新補丁](https://morosedog.gitlab.io/private-lineage-20210806-private-lineage-25)
- <font size="4"><font color="blue">**進階教學**</font>
  - [Java/MySQL 學習資源](https://morosedog.gitlab.io/private-lineage-20210807-private-lineage-26)
  - [IDE 是什麼？](https://morosedog.gitlab.io/private-lineage-20210808-private-lineage-27)
  - Eclipse：
    - [01. Eclipse IDE 安裝](https://morosedog.gitlab.io/private-lineage-20210809-private-lineage-28)
    - [02. Eclipse IDE 簡單介紹](https://morosedog.gitlab.io/private-lineage-20210810-private-lineage-29)
    - [03. Eclipse IDE 調整字型大小](https://morosedog.gitlab.io/private-lineage-20210811-private-lineage-30)
    - [04. Eclipse 匯入天堂私服原始碼](https://morosedog.gitlab.io/private-lineage-20210812-private-lineage-31)
    - [05. Eclipse 原始碼編譯與錯誤排除](https://morosedog.gitlab.io/private-lineage-20210813-private-lineage-32)
    - [06. Eclipse 編輯程式碼和編譯Jar並執行](https://morosedog.gitlab.io/private-lineage-20210814-private-lineage-33)
  - IntelliJ IDEA：
    - [01. IntelliJ IDEA 安裝](https://morosedog.gitlab.io/private-lineage-20210901-private-lineage-34)
    - [02. IntelliJ IDEA 簡單介紹](https://morosedog.gitlab.io/private-lineage-20210902-private-lineage-35)
    - [03. IntelliJ IDEA 進階介紹](https://morosedog.gitlab.io/private-lineage-20210903-private-lineage-36)
    - [04. IntelliJ IDEA 匯入天堂私服原始碼](https://morosedog.gitlab.io/private-lineage-20210904-private-lineage-37)
    - [05. IntelliJ IDEA 原始碼編譯與錯誤排除](https://morosedog.gitlab.io/private-lineage-20210905-private-lineage-38)
    - [06. IntelliJ IDEA 編輯程式碼和編譯Jar並執行](https://morosedog.gitlab.io/private-lineage-20210906-private-lineage-39)
    - [07. IntelliJ IDEA 鑲嵌提示 Java 程式碼的使用與繼承](https://morosedog.gitlab.io/private-lineage-20210909-private-lineage-42)
    - [08. IntelliJ IDEA 逐步除錯(Debug)的步驟與演練](https://morosedog.gitlab.io/private-lineage-20210910-private-lineage-43)
    - [09. IntelliJ IDEA 天堂模擬器除錯(Debug)](https://morosedog.gitlab.io/private-lineage-20210911-private-lineage-44)
    - [10. IntelliJ IDEA 遠端除錯(Remote Debug)Jar包](https://morosedog.gitlab.io/private-lineage-20210912-private-lineage-45)
    - [11. IntelliJ IDEA 反編譯 Jar包](https://morosedog.gitlab.io/private-lineage-20210916-private-lineage-49)
- <font size="4"><font color="red">**核心分析/修改**</font>
<font size="3"></br><開始前，請務必具備基礎的`Java`與`SQL`能力和**<u>進階教學`IntelliJ IDEA`</u>**的[07](https://morosedog.gitlab.io/private-lineage-20210909-private-lineage-42)、[08](https://morosedog.gitlab.io/private-lineage-20210910-private-lineage-43)、[09](https://morosedog.gitlab.io/private-lineage-20210911-private-lineage-44)基本除錯能力></font>
  - 「L1J版」：
    </br><font size="2" color="blue"><b><前五篇適合超級新手學習入門，一步一步非常仔細分析教學></b></font>
    - [人物出生道具分析/修改 (一)](https://morosedog.gitlab.io/private-lineage-20210907-private-lineage-40)
    - [人物出生道具分析/修改 (二)](https://morosedog.gitlab.io/private-lineage-20210908-private-lineage-41)
    - [遊戲帳號分析/Debug (一)](https://morosedog.gitlab.io/private-lineage-20210913-private-lineage-46)
    - [遊戲帳號分析/Debug (二)](https://morosedog.gitlab.io/private-lineage-20210914-private-lineage-47)
    - [遊戲帳號分析/Debug (三)](https://morosedog.gitlab.io/private-lineage-20210915-private-lineage-48)
    </br><font size="2" color="green"><b><學習之初：GM指令的分析/修改></b></font>
    - [GM指令的程式碼邏輯分析](https://morosedog.gitlab.io/private-lineage-20210917-private-lineage-50)
    - [GM指令分析 (全輔助)](https://morosedog.gitlab.io/private-lineage-20210918-private-lineage-51)
    - [GM指令/一般指令分析 (Who)](https://morosedog.gitlab.io/private-lineage-20210919-private-lineage-52)
    - [GM指令分析/修改 (怪物血條)](https://morosedog.gitlab.io/private-lineage-20210920-private-lineage-53)
    - [GM指令分析/修改 (描述)](https://morosedog.gitlab.io/private-lineage-20210921-private-lineage-54)
    - [GM指令分析/修改 (金幣)](https://morosedog.gitlab.io/private-lineage-20211015-private-lineage-55)
    - [GM指令分析 (創立道具)](https://morosedog.gitlab.io/private-lineage-20211016-private-lineage-56)
    - [GM指令分析 (創立套裝)](https://morosedog.gitlab.io/private-lineage-20211017-private-lineage-57)
    - [GM指令分析 (贈送)](https://morosedog.gitlab.io/private-lineage-20211018-private-lineage-58)
    - [GM指令分析 (限等贈送)](https://morosedog.gitlab.io/private-lineage-20211019-private-lineage-59)
    - [GM指令分析 (移動)](https://morosedog.gitlab.io/private-lineage-20211020-private-lineage-60)
    - [GM指令分析 (房間)](https://morosedog.gitlab.io/private-lineage-20211021-private-lineage-61)
    - [GM指令分析 (前往玩家)](https://morosedog.gitlab.io/private-lineage-20211022-private-lineage-62)
    - [GM指令分析 (召回玩家)](https://morosedog.gitlab.io/private-lineage-20211023-private-lineage-63)
    - [GM指令分析 (前往怪物)](https://morosedog.gitlab.io/private-lineage-20211024-private-lineage-64)
    - [GM指令分析 (召喚怪物)](https://morosedog.gitlab.io/private-lineage-20211025-private-lineage-65)
    - [GM指令分析 (召喚寵物)](https://morosedog.gitlab.io/private-lineage-20211026-private-lineage-66)
    - [GM指令分析 (創怪/創NPC)](https://morosedog.gitlab.io/private-lineage-20211027-private-lineage-67)
- <font size="4"><font color="#EE7700">**補丁介紹/說明**</font>
  - [客戶端idx、pak說明](https://morosedog.gitlab.io/private-lineage-20220201-private-lineage-68)
  - [補丁副檔名對應說明](https://morosedog.gitlab.io/private-lineage-20220202-private-lineage-69)
  - [補丁吃檔資料夾對應](https://morosedog.gitlab.io/private-lineage-20220203-private-lineage-70)
- <font size="4"><font color="#E63F00">**工具介紹/使用**</font>
  - [eat (吃檔教學)](https://morosedog.gitlab.io/private-lineage-20220204-private-lineage-71)
  </br><font size="2" color="green"><b><瀏覽/抽檔工具></b></font>
  - [PakViewer 介紹](https://morosedog.gitlab.io/private-lineage-20220205-private-lineage-72)
  - [Pakext 工具](https://morosedog.gitlab.io/private-lineage-20220206-private-lineage-73)
  - [PakViewe 工具](https://morosedog.gitlab.io/private-lineage-20220207-private-lineage-74)
  - [PakViewer Ver.3.0 工具](https://morosedog.gitlab.io/private-lineage-20220208-private-lineage-75)
  - [PackViewer_beta2 工具](https://morosedog.gitlab.io/private-lineage-20220209-private-lineage-76)
  - [L1Viewer 工具](https://morosedog.gitlab.io/private-lineage-20220210-private-lineage-77)
  - [LineageSpr 工具](https://morosedog.gitlab.io/private-lineage-20220211-private-lineage-78)
  - [Lineage Icon v120119 工具](https://morosedog.gitlab.io/private-lineage-20220212-private-lineage-79)
  - [MTools 工具](https://morosedog.gitlab.io/private-lineage-20220213-private-lineage-80)
  </br><font size="2" color="green"><b><加解密工具></b></font>
  - [XML加解密 工具](https://morosedog.gitlab.io/private-lineage-20220214-private-lineage-81)
  - [SPZ、XML加解密 工具](https://morosedog.gitlab.io/private-lineage-20220215-private-lineage-82)
  - [對話檔加密解密 工具](https://morosedog.gitlab.io/private-lineage-20220216-private-lineage-83)
  </br><font size="2" color="green"><b><登入器素材工具></b></font>
  - [登入器素材抽檔 工具](https://morosedog.gitlab.io/private-lineage-20220217-private-lineage-84)
  </br><font size="2" color="green"><b><轉檔工具></b></font>
  - [TBT編譯器 工具(PNG↔TBT)](https://morosedog.gitlab.io/private-lineage-20220218-private-lineage-85)
  - [Linskin4.04 工具(IMG↔BMP)](https://morosedog.gitlab.io/private-lineage-20220219-private-lineage-86)
  - [SPR-BMP互轉 工具(SPR↔BMP)](https://morosedog.gitlab.io/private-lineage-20220220-private-lineage-87)
  </br><font size="2" color="green"><b><圖檔工具></b></font>
  - [SFDviewer 工具(圖檔座標定位)](https://morosedog.gitlab.io/private-lineage-20220221-private-lineage-88)
  - [ViX 工具(圖檔轉位元)](https://morosedog.gitlab.io/private-lineage-20220501-private-lineage-96)
  </br><font size="2" color="green"><b><地圖工具></b></font>
  - [超簡易地圖預覽 工具](https://morosedog.gitlab.io/private-lineage-20220222-private-lineage-89)
  - [Lineage Map V1 工具](https://morosedog.gitlab.io/private-lineage-20220223-private-lineage-90)
  - [地圖屬性修改 工具](https://morosedog.gitlab.io/private-lineage-20220224-private-lineage-91)
  - [LiTo Map 工具](https://morosedog.gitlab.io/private-lineage-20220225-private-lineage-92)
  </br><font size="2" color="green"><b><檔名工具></b></font>
  - [Flexible Renamer 工具(批量修改檔名)](/private-lineage-20220502-private-lineage-97)
- <font size="4"><font color="#CC0000">**對話檔分析/修改**</font>
  - [NPC對應對話檔分析](https://morosedog.gitlab.io/private-lineage-20220226-private-lineage-93)
  - [文字對話檔分析](https://morosedog.gitlab.io/private-lineage-20220227-private-lineage-94)
  - [圖片對話檔分析](https://morosedog.gitlab.io/private-lineage-20220228-private-lineage-95)
  - [跳轉其他對話檔分析<Link篇>](https://morosedog.gitlab.io/private-lineage-20220503-private-lineage-98)
  - [跳轉其他對話檔分析<Action篇>](https://morosedog.gitlab.io/private-lineage-20220504-private-lineage-99)
  - [執行行動分析<強化魔法師篇>](https://morosedog.gitlab.io/private-lineage-20220505-private-lineage-100)
  - [執行行動分析<傳送師篇>](https://morosedog.gitlab.io/private-lineage-20220506-private-lineage-101)
  - [執行行動分析<道具篇>](https://morosedog.gitlab.io/private-lineage-20220507-private-lineage-102)
- <font size="4"><font color="#C10066">**變檔分析/修改**</font>
  - [變身檔新增修改<快速入門>](https://morosedog.gitlab.io/private-lineage-20220508-private-lineage-103)
  </br><font size="2" color="green"><b><初階教學與知識></b></font>
  - [GM指令使用 (影像動畫)](https://morosedog.gitlab.io/private-lineage-20220509-private-lineage-104)
  - [GM指令使用 (人物變身)](https://morosedog.gitlab.io/private-lineage-20220510-private-lineage-105)
  - [客戶端和登入器與變身檔關係分析](https://morosedog.gitlab.io/private-lineage-20220511-private-lineage-106)
  - [變身檔與 gfxid、polyid 分析](https://morosedog.gitlab.io/private-lineage-20220512-private-lineage-107)
  - [資料庫中 gfxid、polyid 分析](https://morosedog.gitlab.io/private-lineage-20220513-private-lineage-108)
  - [登入器的 spr_action 產生](https://morosedog.gitlab.io/private-lineage-20220514-private-lineage-109)
  - [資料庫中 spr_action 分析](https://morosedog.gitlab.io/private-lineage-20220515-private-lineage-110)
  - [動畫圖檔 spr 基礎了解說明](https://morosedog.gitlab.io/private-lineage-20220516-private-lineage-111)
  </br><font size="2" color="orange"><b><進階教學與知識></b></font>
  - [變身檔-初步說明與規則](https://morosedog.gitlab.io/private-lineage-20220517-private-lineage-112)
  - [變身檔-格式與編碼基礎](https://morosedog.gitlab.io/private-lineage-20220518-private-lineage-113)
  - [變身檔-物件分辨的教學](https://morosedog.gitlab.io/private-lineage-20220519-private-lineage-114)
  - [變身檔-濾鏡效果的教學](https://morosedog.gitlab.io/private-lineage-20220520-private-lineage-115)
  - [變身檔-附加物件的教學](https://morosedog.gitlab.io/private-lineage-20220521-private-lineage-116)
  - [變身檔-武器指令的教學](https://morosedog.gitlab.io/private-lineage-20220522-private-lineage-117)
  - [變身檔-魔法效果的教學](https://morosedog.gitlab.io/private-lineage-20220523-private-lineage-118)
  - [變身檔-加速指令的教學](https://morosedog.gitlab.io/private-lineage-20220524-private-lineage-119)
  - [變身檔-走路分析與修改](https://morosedog.gitlab.io/private-lineage-20220525-private-lineage-120)
  - [變身檔-攻擊分析與修改](https://morosedog.gitlab.io/private-lineage-20220526-private-lineage-121)
  - [變身檔-施法分析與修改](https://morosedog.gitlab.io/private-lineage-20220527-private-lineage-122)
  - [變身檔-僵直分析與修改](https://morosedog.gitlab.io/private-lineage-20220528-private-lineage-123)
  - [變身檔-撿取分析與修改](https://morosedog.gitlab.io/private-lineage-20220529-private-lineage-124)
  - [變身檔-指向指令分析與修改](https://morosedog.gitlab.io/private-lineage-20220530-private-lineage-125)
- <font size="4"><font color="#F06E52">**XML分析/教學**</font>
  - [XML 基礎教學](https://morosedog.gitlab.io/xml-20221101-XML-0/#%E6%95%99%E5%AD%B8%E7%AB%A0%E7%B5%90)
  - 🔒[JAXB 基礎](https://morosedog.gitlab.io/private-lineage-20230117-private-lineage-126)
  - 🔒[Java DOM 基礎](https://morosedog.gitlab.io/private-lineage-20230205-private-lineage-129)
  - <font size="4" color="orange"><b><Server端></b></font>
    - 「L1J版」：
      - 🔒[XML 檔案清單說明](https://morosedog.gitlab.io/private-lineage-20230118-private-lineage-127)
      - 🔒[BOSS 重生設定分析 (BossCycle)](https://morosedog.gitlab.io/private-lineage-20230127-private-lineage-128)
      - 🔒<s>[GM 指令設定分析 (GMCommands)]</s>
      - 🔒<s>[寶盒設定分析 (TreasureBox)]</s>
      - 🔒<s>[物品製作設定分析 (ItemMaking)]</s>
      - 🔒<s>[單品製作設定分析 (SingleItemMaking)]</s>
      - 🔒<s>[任務設定分析 (Quest)]</s>
      - 🔒<s>[傳送師設定分析 (Teleporter)]</s>
  - <font size="4" color="blue"><b><Client端></b></font>
    - <s>[coming soon]</s>

## 分享 

如有需要分享掛載，這邊提供動態圖：
![](https://morosedog.gitlab.io/images/private-lineage/chapter0/morosedog.gif)

感謝各大技術論壇友情分享：
- [Linhelper論壇](https://bbs.linhelper.com/?fromuid=683)

## 結語

- 2022-05-31：**<u>發現文章被惡意複製盜連，且未用任何形式的轉載註明出處</u>**。<font color="red"><**已與`Google`申請版權內容撤除要求**></font>
- 2022-06-01：**<font color="blue">將保持<u>既有的文章</u>「直接閱讀」</font>**。
- 2022-06-03：**<font color="blue"><u>新研究技術文章</u>會「<s>繼續分享</s>」</font>**，<font color="red"><s>Why? 要讓更多人學習<u>避免購買版本</s></u></font>。
- 2023-01-17：**<font color="blue">不定時不定期，緩慢更新文章</font>**，較為深入的分析與技術將會對其文章做加密，**<font color="red">避免</font>**再次被**<font color="red">「惡意複製盜連」</font>**。
- 2023-01-18：**<font color="red">如何取得🔑文章密碼？</font>**<font color="#FFFFF">僅自行閱讀…</font>
- 2023-05-29：發現**<font color="red">持續惡意複製盜連文章</font>**，將不會依任何免費形式繼續分享天堂私服教學。
