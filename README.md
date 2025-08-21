# rime-ms-quick
rime 輸入法 (https://rime.im/) 的微軟傳統排位速成方案


### 微軟傳統速成輸入法

* 按微軟速成固定排位
* 沒有聯想字
* 不會自組字詞

供習慣使用微軟傳統速成，沒有使用聯想字的用家使用。因為 rime 等開源輸入法，可將微軟傳統速成輸入法選字習慣用於不同平台，例如 MacOS、Android。相關資料可參見以下


#### 使用這個方案請參見以下

Windows (參考專案 : https://github.com/rime/weasel )

1. 安裝軟件後，下載此專案的兩個 `yaml` 檔案 ( `ms_quick.dict.yaml` 和 `ms_quick.schema.yaml` )
2. 把檔案放入小狼亳安裝路徑的 \data 裡面
3. 再點擊 「【小狼毫】輸入法設定」，選擇「微軟速成」

Android (參考專案 : https://github.com/osfans/trime )

1. 手機 google play 安裝 同文輸入法 (google play 已下架。此方案是適配 3.1.3 版本，可以在 github 下載: [版本 3.1.3](https://github.com/osfans/trime/releases/download/3.1.3/trime-3.1.3-20190930.apk))
2. 將兩個 `yaml` 檔案 ( `ms_quick.dict.yaml` 和 `ms_quick.schema.yaml` )，連同 `Android/trime.custom.yaml`，放到 Android 系統的 /rime 目錄中
3. 打開 同文輸入法 設置，點擊 「輸入/方案」，勾選「傳統速成」
4. 回到 同文輸入法 設置的根目錄，點擊「部署」
5. 部署後如果打中文有閃退，出現不了候選字懸浮窗，可以在同文輸入設置 -> 鍵盤，先關掉「顯示懸浮窗口」，轉應用打一下字，再回到設置將「顯示懸浮窗口」重新打開，就會正常


MacOS  (參考專案 : https://github.com/rime/squirrel )

Lunix (參考專案 : https://github.com/rime/ibus-rime )

#### 繁簡輸入位置不同問題解決

可以將 opencc/ 的兩個檔案複製到 \data\opencc\ 中，這是將本來 opencc 中繁轉簡「一對多」都改成「一對一」，這樣轉了簡體輸入後，速度的候選字排位仍能保持一致