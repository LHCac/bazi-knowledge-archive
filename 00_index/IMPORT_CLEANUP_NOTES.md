# 壓縮檔匯入整理紀錄

## 匯入來源

- 原始檔：`bazi-standalone.zip`
- 保存位置：`99_sources/imports/bazi-standalone.zip`
- 整理分支：`agent/unpack-bazi-archive`

## 已完成處理

1. 將壓縮檔內的正式八字資料夾展開至 repository 根目錄。
2. 保留原始 ZIP，作為來源追溯與重新驗證依據。
3. 移除 `liuyao-divination-archive-export-bazi-standalone/` 巢狀目錄。
4. 該巢狀目錄內的 Markdown 檔案，經 SHA-256 檢查皆與根目錄版本完全相同，因此移除不影響內容。
5. 語意相近但內容不完全相同的文件未自動合併，避免誤刪規則或來源差異。

## 後續建議

- 補齊 `00_index/` 的十神、格局、行運、問事與案例子索引。
- 對含有重斷語的十神宮位文件建立「降火修正版」。
- 為來源文件補充書名、章節、頁碼或網址等可追溯資料。
- 語意重疊文件應先比較差異，再由人工決定合併或保留。
