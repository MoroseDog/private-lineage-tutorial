## 前言

天堂私服架設教學、研究、核心修改、資料庫修改；天堂私服從無到有，手把手教學，簡單易懂輕鬆上手。

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
- <font size="4"><font color="red">**核心分析/修改**</font>
<font size="3"><開始前，請務必具備基礎的`Java`與`SQL`能力和**<u>進階教學`IntelliJ IDEA`</u>**的[07](/private-lineage-20210909-private-lineage-42)、[08](/private-lineage-20210910-private-lineage-43)、[09](/private-lineage-20210911-private-lineage-44)基本除錯能力></font>
  - 「L1J版」：
    <font size="2" color="blue"><b><前五篇適合超級新手學習入門，一步一步非常仔細分析教學></b></font>
    - [人物出生道具分析/修改 (一)](https://morosedog.gitlab.io/private-lineage-20210907-private-lineage-40)
    - [人物出生道具分析/修改 (二)](https://morosedog.gitlab.io/private-lineage-20210908-private-lineage-41)
    - [遊戲帳號分析/Debug (一)](https://morosedog.gitlab.io/private-lineage-20210913-private-lineage-46)
    - [遊戲帳號分析/Debug (二)](https://morosedog.gitlab.io/private-lineage-20210914-private-lineage-47)
    - [遊戲帳號分析/Debug (三)](https://morosedog.gitlab.io/private-lineage-20210915-private-lineage-48)
      
    <font size="2" color="green"><b><學習之初：GM指令的分析/修改></b></font>
      
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
    - [GM指令分析 (前往怪物)](https://morosedog.gitlab.io//private-lineage-20211024-private-lineage-64)
    - [GM指令分析 (召喚怪物)](https://morosedog.gitlab.io//private-lineage-20211025-private-lineage-65)
    - [GM指令分析 (召喚寵物)](https://morosedog.gitlab.io//private-lineage-20211026-private-lineage-66)
    - [GM指令分析 (創怪/創NPC)](https://morosedog.gitlab.io//private-lineage-20211027-private-lineage-67)
    - ....
  - 「YiWei版」：
    - ....
- <font size="4"><font color="rosybrown">**工具介紹/使用**</font>
  - ....
- <font size="4"><font color="chocolate">**圖檔分析/修改**</font>
  - ....
- <font size="4"><font color="saddlebrown">**輔助開發**</font>
  - ....    
  
## 分享 

如有需要分享掛載，這邊提供動態圖：

![](https://morosedog.gitlab.io/images/private-lineage/chapter0/morosedog.gif)


感謝各大技術論壇友情分享：
- [Linhelper論壇](https://bbs.linhelper.com/?fromuid=683)


## 結語
以上的章節只是我初步的規劃，當然有可能增/刪/改，且章結順序並不一定代表撰寫的順序；
但我這邊會盡量依照順序去撰寫，畢竟這個順序是學習的一個優先順序。

建議大家針對其順序去做學習研究~~。
