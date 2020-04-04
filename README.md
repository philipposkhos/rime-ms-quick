# rime-ms-quick
rime 輸入法 (https://rime.im/) 的微軟傳統排位速成方案


### 微軟傳統速成輸入法

* 按微軟速成固定排位
* 沒有聯想字
* 不會自組字詞

>不足 : 當直接輸入單字碼字時(例如 手, 火等)，無法像 Windows 輸入法那樣直接用 space 輸入，需要像選字那樣按 1 字。如有解決的建議，麻煩留言。



供習慣使用微軟傳統速成，沒有使用聯想字的用家使用。因為 rime 等開源輸入法，可將微軟傳統速成輸入法選字習慣用於不同平台，例如 MacOS、Android。相關資料可參見以下


#### 使用這個方案請參見以下

Windows (參考專案 : https://github.com/rime/weasel )

1. 安裝軟件後，下載此專案的兩個 yaml 檔案 ( `ms_quick.dict.yaml` 和 `ms_quick.schema.yaml` )
2. 把檔案放入小狼亳安裝路徑的 \data 裡面
3. 再點擊 「【小狼毫】輸入法設定」，選擇「微軟速成」

Android (參考專案 : https://github.com/osfans/trime )

1. 手機 google play 安裝 同文輸入法
2. 將兩個 `yaml` 檔案 ( `ms_quick.dict.yaml` 和 `ms_quick.schema.yaml` )，連同 `Android/trime.yaml`，放到 Android 系統的 /rime 目錄中，同時覆蓋應用原本的 `trime.yaml`。
(`trime.yaml` 是手機鍵盤佈局檔，如果本來 `trime.yaml` 檔案是有改過的的，可以把此專案 `Android/trime.yaml` 檔裡最底部 ms_quick block 貼到自己的 `trime.yaml` 中)
3. 打開 同文輸入法 設置，點擊 「輸入/方案」，勾選「傳統速成」
4. 回到 同文輸入法 設置的根目錄，點擊「部署」


MacOS  (參考專案 : https://github.com/rime/squirrel )

Lunix (參考專案 : https://github.com/rime/ibus-rime )