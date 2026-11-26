# Mouse Hub Plugins

社群插件市集。每個插件是一個 JSON 宣告檔，定義裝置的 HID 讀取規則。

## 安裝方式

在 Mouse Hub 的「市集」分頁瀏覽並一鍵安裝，或手動把 JSON 放進 `plugins/` 目錄。

## 提交插件

1. Fork 本 repo
2. 在 `plugins/` 新增你的 JSON（參考 `plugins/example-mouse.json`）
3. 更新 `marketplace.json` 加入你的插件
4. 發 PR

## 安全

- 插件是**宣告式 JSON**，不執行任何程式碼
- 只允許 HID 讀取規則（Output Report / Feature Report）
- 格式不符的插件會被拒絕安裝

## 市集索引

`marketplace.json` 列出所有可安裝的插件。