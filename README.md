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

兩個版本的**方案／詞庫相同**（`ms_quick.schema.yaml`、`ms_quick.dict.yaml`），差在鍵盤設定檔，請依同文版本選資料夾，**不要混用**。

共用步驟：把檔案放到同文「用戶資料夾」根目錄（舊版常見路徑是 `/sdcard/rime`；3.3 請到同文設定查看「用戶資料夾」），勾選方案「傳統速成」，再部署。

##### 同文 3.1.3

適配檔在 `Android/3.1.3/`。Google Play 已下架，可在 GitHub 下載：[3.1.3 APK](https://github.com/osfans/trime/releases/download/3.1.3/trime-3.1.3-20190930.apk)

1. 複製 `ms_quick.dict.yaml`、`ms_quick.schema.yaml`，以及 `Android/3.1.3/trime.custom.yaml`
2. 放到用戶資料夾根目錄（只要 `trime.custom.yaml` 這個檔名，不要連 `Android/3.1.3/` 資料夾一起放）
3. 同文設置 → 輸入／方案，勾選「傳統速成」
4. 回到設置根目錄，點「部署」
5. 若打中文閃退、候選懸浮窗出不來：設置 → 鍵盤，先關掉「顯示懸浮窗口」，換應用打一下字，再打開該選項

##### 同文 3.3

適配檔在 `Android/3.3/`。3.1.3 的 `trime.custom.yaml` 在 3.3 **不能用**（舊懸浮窗／鍵盤格式已失效），請改用獨立主題。

1. 複製 `ms_quick.dict.yaml`、`ms_quick.schema.yaml`，以及 `Android/3.3/ms_quick.trime.yaml`
2. 放到用戶資料夾根目錄（只要 `ms_quick.trime.yaml` 這個檔名，不要連 `Android/3.3/` 資料夾一起放）
3. 同文設置 → 鍵盤樣式 → 主題，選「傳統速成」（鍵盤佈局綁在主題上，配色只能選這個主題裡有的）
4. 必須要打開候選視窗 (同文設置 → 候選視窗，選始終顯示)，才能見到候選字，並用 空白鍵 翻頁
5. 方案勾選「傳統速成」，然後部署

MacOS  (參考專案 : https://github.com/rime/squirrel )

Linux (參考專案 : https://github.com/rime/ibus-rime )

#### 繁簡輸入位置不同問題解決

可以將 opencc/ 的兩個檔案複製到 \data\opencc\ 中，這是將本來 opencc 中繁轉簡「一對多」都改成「一對一」，這樣轉了簡體輸入後，速度的候選字排位仍能保持一致