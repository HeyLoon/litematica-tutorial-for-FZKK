# Litematica(投影)模組使用教學
## 前言
"生電"為本服的特色玩法之一，所謂"生電"即是**生存電路**的簡稱。應本服大部分人皆非紅石電路方面專家，但又想體驗(~~被勞役~~)建造紅石電路的快感，故撰本篇教學如何使用/安裝投影模組。
## 一. 前置作業-模組載入器
Litematica模組目前只支援**Fabric**，所以首先必須安裝Fabric
[Fabric下載網址點我](https://fabricmc.net/use/installer/)
相信各位一中南女的優秀青年一定知道下載的英文是什麼
下載完打開應該會看到這個介面，照著我這圖片改就好:
![](https://i.imgur.com/h6bJTE0.png)
改完後就點安裝即可，顯示successfully installed後即可關閉
重新打開Minecraft Launcher後，應該會看到這個畫面
![](https://i.imgur.com/VWH8LLl.png)
右下角多了Fabric Loader，先打開一次遊戲，然後可以先關掉(為了讓mod資料夾產生出來)
## 二. 前置模組及本體安裝
Litematica需要安裝**MaLiLib library**以及**Fabric API**
這邊都幫各位準備好了，點進去後下載即可
1.19.3: 
[litematica-fabric-1.19.3-0.13.1.jar](https://xpsv5-my.sharepoint.com/:u:/g/personal/heyloon_xpsv5_onmicrosoft_com/EUEHSciLOWpIpPng0DQAGiUBljonwUphWkm2bqPC1RITTQ?e=E4YTl2)
[malilib-fabric-1.19.3-0.14.0.jar](https://xpsv5-my.sharepoint.com/:u:/g/personal/heyloon_xpsv5_onmicrosoft_com/EZKu9X5224dGncYn7rLk6xsBXHFW_i_KhgPn_Pq_uzqSeQ?e=jENohQ)
[fabric-api-0.73.0+1.19.3.jar](https://xpsv5-my.sharepoint.com/:u:/g/personal/heyloon_xpsv5_onmicrosoft_com/ETbFbi5YtgdOhqkln3TmDIQBEVSTFo_pvHL1w9x6wUUQJg?e=hK3wSw)
下載完後會得到這樣三個檔案
![](https://i.imgur.com/CzbSYRv.png)
接著把這兩個檔案複製/剪下後
在導航欄輸入%appdata%
![](https://i.imgur.com/RwJzxOJ.png)
按下enter，進入.minecraft資料夾，你會看到:
![](https://i.imgur.com/Q95BedR.png)
進入mods資料夾，把三個模組貼上，就大功告成了!
## 三. 開始使用
本文全程使用英文版Litematica，如果需要中文翻譯包請見附錄一
首先先按下**m開啟面板**，你應該會看到以下頁面:
![](https://i.imgur.com/ZqoXMQ9.jpg)
首先我們先進行首次使用的基礎設定。
### 甲.首次設定
先進入**Configuration menu**
選到**easyPlaceToggle**
![](https://i.imgur.com/vnr6WcK.jpg)
此功能為**切換到快速放置模式**，建議設定為x
~(快速放置模式可以讓Litematica直接使用你背包內的東西放到投影出的藍圖上，材料備夠了就只要無腦放置就好)~
接著選到**toolItem**
![](https://i.imgur.com/jBqIbWN.jpg)
預設為木棒，覺得麻煩可以改為其他物品
至此，基礎設定完成
### 乙. 選取投影
這個部分其實是寫完之後想到要加的，所以可能跟下段有接不起來的感覺，敬請見諒。
首先先進到你想複製的建築所在的地圖，這邊以迪克島的超巨型迪克為例:
先拿著預設工具，**按著ctrl**使用滾輪滾到Mode[1/9]:Area Selection的部分
![](https://i.imgur.com/wOaEbRc.jpg)
以右鍵為第一點，左鍵為第二點，框出想要投影的區域，框完應該長這樣:
![](https://i.imgur.com/2ErTBAm.jpg)
然後按下m，進入到Area Editor
![](https://i.imgur.com/sMQ9eXS.png)
應該會看到這個介面:
![](https://i.imgur.com/CnzJaZA.jpg)
Selection name和Sub-region box name可以調整分區名字，但一般狀態下我們用不到，無須更改，Corner1,2為兩點座標，對過正確即可，接著按下Save Schematic，應該會看到以下畫面:
![](https://i.imgur.com/ZsPo7G0.png)
此時上面框框才需改成自己想要的名字，下面三個可勾選選項分別為: 只顯示可見物體(不包含屏障、半透明物品)、從(一般)藍圖保存、無視實體(蝙蝠、村民等生物)
接著按下保存，就會自動存到`%appdata%\.minecraft\schematics`中了!


### 丙. 放置投影
同樣打開UI，選取Load Schematics
![](https://i.imgur.com/SBLPDH2.jpg)
然後你會發現--什麼都沒有:)
因為你必須先將藍圖放到`%appdata%\.minecraft\schematics`裡面
![](https://i.imgur.com/9OhOe7J.png)
> Note: 投影模組的藍圖一定是.litematic檔，不是WorldEdit的.schem檔，不要搞混了!

然後回到UI，點你要的藍圖
![](https://i.imgur.com/HZOZzya.png)
下面幾個按鈕依序是: 載入藍圖、材料列表、顯示已載入藍圖、回到主頁
這邊點**載入藍圖-Load Schematic**
![](https://i.imgur.com/YFvmxhp.jpg)
建築就會出現在你眼前了!
可以使用設定的工具來移動基準點的位置，如果要把基準點崁進地板內的話要蹲下後再按
接著再按m，選擇**Schematic Placements**
![](https://i.imgur.com/ZZCNpAP.jpg)
這邊會顯示你已經載入的藍圖，三個選項依序是: 設定、是否顯示藍圖，卸載藍圖
![](https://i.imgur.com/yalbInz.jpg)
這邊點**Configure**，進入後畫面如下:
![](https://i.imgur.com/rjt8sfb.jpg)
相信各位基礎英文都有學好，所以這邊只介紹一些功能
Rotation是旋轉角度
Mirror是鏡像
Schematic Verifier是檢測有沒有蓋完整的驗證功能
至此，放置投影的部分結束
### 丁. 實裝!
通常放置完成後應該就沒甚麼問題了，所以這邊就分享一些實裝小技巧。
首先在建造較大型的建築時，建議一層一層來建造，預設使用**PageUp**還有**PageDown**來增加/減少顯示層數。
另外，在蓋大型建築時也建議使用材料表功能先導出材料表提前準備，但千萬別準備剛好，常會有悲劇發生。
## 四. 附錄
### 附錄一: 中文版Litematica
這邊提供兩種方式。
#### 1. 使用材質包更改
首先先下載材質包:
[fabric-mod-chinese-traslation-resouce-pack-main.zip](https://xpsv5-my.sharepoint.com/:u:/g/personal/heyloon_xpsv5_onmicrosoft_com/Ec83-DyjFfZGoRpatS03BYIBMMrjs8sn93Rie4zjyDmn5g?e=NZ6yfH)
下載完後會得到一個壓縮包，**不需要解壓**
將壓縮包複製到`.minecraft\resourcepacks`後開啟遊戲
點擊`遊戲目錄`中的`選項`
![](https://i.imgur.com/p1tEkFP.png)
點擊`資源包`
![](https://i.imgur.com/BpY1627.png)
將`fabric-mod-chinese-traslation-resouce-pack-main.zip`點到右方(如果顯示不相容忽略即可)
![](https://i.imgur.com/IPQYF15.png)
然後再點擊m，應該就是繁體中文版了
![](https://i.imgur.com/qBHBbMe.png)
#### 2. 使用RPMTW Patform
這是最一勞永逸的方法，這個模組裝了之後以後所有模組就都不用裝翻譯了。
因為時常更新，所以不直接提供檔案，請先到[RPMTW官網](https://www.rpmtw.com/)
看到自動中文化更新模組，點擊立即下載
![](https://i.imgur.com/BmIuj2i.png)
選擇1.19.3版本，平台選Fabric
![](https://i.imgur.com/zcpce2L.png)
下載下來的檔案，同樣放入`./.minecraft/mods`資料夾即可!
#### 3. RPMTW Platform功能設定
開始使用RPMTW後，應該會看到宇宙通訊之類不想要的功能，這邊提供解法:
先下載Mod Menu模組:
1.19.3: [modmenu-5.0.2.jar](https://xpsv5-my.sharepoint.com/:u:/g/personal/heyloon_xpsv5_onmicrosoft_com/ERSbdQ6pU1dKp1XwNz6KMaEBf7kUF2NYsIoRRVnYj8VK-A?e=sTyx9e)
同樣放入`./.minecraft/mods`資料夾，然後會看到`遊戲目錄`多出一個`模組`
![](https://i.imgur.com/m6zeZcC.png)
點他，選到RPMTW Platform Mod，點及擊右上的這顆按鈕
![](https://i.imgur.com/l3sjyOT.png)
然後就能自行將不要的功能關閉了。
### 附錄二- 進階用法
更深入的使用，可以參考:
[Anyone can help me. How do I make schematics with litematica 1.14.4 - Reddit](https://old.reddit.com/r/Minecraft/comments/cqdmkk/anyone_can_help_me_how_do_i_make_schematics_with/exeug78/)
[maruohon/litematica-wiki - Github
](https://github.com/maruohon/litematica/wiki)
### 附錄三- 來源
本文參考/引用了以下網頁之內容(A-Z)
[Fabric](https://fabricmc.net/)
[Fabric API](https://github.com/FabricMC/fabric)
[MaLiLib](https://www.curseforge.com/minecraft/mc-mods/malilib)
[Mod Menu](https://github.com/TerraformersMC/ModMenu)
[Mod Menu Wiki](https://github.com/TerraformersMC/ModMenu/wiki/API)

##### 最後校稿by 黑輪HeyLoon 2023.1.30 01:00, 有問題歡迎洽DC: 黑輪#1198