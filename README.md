# 衛福部機構公開資訊

提供醫事機構的床數、服務項目、診療科別、基本資訊等資料。

## 2015-05-10

突然發現健保署的網站新增了兩個資料，分別是**醫療院所服務項目**跟**醫療院所診療科別**。

由於健保署的官方資料會比我從**衛生福利部醫事機構評鑑公開資訊網站**上爬的資料 (也就是下面的 Hospital-Dept.csv) 要來的正確，故建議有需要可以改用新的官方資料。

## 資料來源與檔案說明

1. [衛生福利部醫事機構評鑑的公開資訊網站] (http://mcia.mohw.gov.tw/openinfo)
  * **Hospital-BedSize.csv** - 醫事機構病床類別與床數資料
  * **Hospital-Dept.csv** - 醫事機構診療科別資料

2. [衛生福利部中央健保署特約醫事機構資料] (http://www.nhi.gov.tw/webdata/webdata.aspx?menu=18&menu_id=703&webdata_id=660)
  * **hospbsc.csv** - 健保特約醫療院所名冊含機構代碼、地址、電話、特約類別 (2015-05-08)
  * **service.csv** - 醫療院所服務項目 (2015-05-08) NEW!
  * **detafunc.csv** - 醫療院所診療科別 (2015-05-08) NEW!
  * **1290_1_hosp_code.csv** - 型態別代碼對照檔 (2015-05-08)
  * **1292_1_service_code.csv** - 服務項目代碼對照檔 (2015-05-08)
  * **1293_1_func_type.csv** - 診療科別代碼對照檔 (2015-05-08)

## 資料欄位說明

* 醫事機構病床類別與床數資料
```
City: 縣市
Area: 鄉鎮
Name: 醫事機構名稱
Zone: 院區別
特約類別: 此欄位已經過整理，與醫事機構特約類別代碼對照後回復為類別文字。
機構屬性名稱：此欄位已經過整理，與醫事機構種類代碼對照後回復為屬性名稱。
病床類別
病床名稱
病床數量
```

* 醫事機構診療科別資料
```
BAS_AGENCY_ID: 醫事機構代碼
Name: 醫事機構名稱
Zone: 院區別
City: 縣市
Area: 鄉鎮
BAS_SEQ: 網址內有但不確定意義
ZONE_SEQ: 網址內有但不確定意義
ZONE_CODE: 特約類別
Department Name: 診療科別
```

## 代碼對照

型態別、服務項目以及診療科別請參考對照檔，其餘則列示如下：

* 業務組別對照
```
業務組別,業務組名稱
"1","臺北業務組"
"2","北區業務組"
"3","中區業務組"
"4","南區業務組"
"5","高屏業務組"
"6","東區業務組"
```

* 特約類別代碼對照檔
```
特約類別,特約類別說明
"1","醫學中心"
"2","區域醫院"
"3","地區醫院"
"4","診所"
"5","藥局"
"6","居家護理"
"7","康復之家"
"8","助產所"
"9","檢驗所"
"A","物理治療所"
"B","特約醫事放射機構"
"X","不詳"
```

## 資料更新日期

本資料擷取日期為 2015-05-08

## 授權

本資料採用 [CC0 1.0 公眾領域貢獻宣告] (https://creativecommons.org/publicdomain/zero/1.0/deed.zh_TW)
