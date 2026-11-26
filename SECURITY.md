# Mouse Hub Plugins Registry

社群市集索引：https://raw.githubusercontent.com/mouse-hub/plugins/main/marketplace.json

## 格式

每個插件是 JSON 宣告檔，定義：
- `name`, `version`, `vid`, `pid`, `device_type`
- `read`: battery / dpi / poll_rate 的讀取規則

## 安全模型

- **不執行任何程式碼** — 純宣告式
- 只允許 `output_report` / `feature_report` 兩種讀取方法
- 安裝時驗證 JSON schema，格式不符直接拒絕
- 惡意插件無法存取檔案系統、網路或執行命令