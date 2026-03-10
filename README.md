# 🥟 悉尼餃子店 - AI 電話訂餐自動化方案

> **Sydney Dumpling House - AI Phone Order Automation**

自動化電話訂單處理系統，解決老闆開車時無法接英文電話的痛點。

## 🔗 線上預覽

- 📊 **完整 Dashboard**: https://你的用戶名.github.io/你的倉庫名/dumpling_dashboard.html
- 🎬 **快速演示**: https://你的用戶名.github.io/你的倉庫名/dumpling_presentation.html

## 🎯 解決的問題

- ❌ 老闆是「人肉中轉站」：英文電話 → 理解 → 翻譯 → 通知廚房（15分鐘延誤）
- ❌ 語言切換疲勞：聽力 + 轉述，準確率僅 85%
- ❌ 錯過來電：開車時無法接單，損失生意

## ✅ 解決方案

**AI 電話接線員 → 自動翻譯 → 微信通知**

### 架構
```
顧客電話 → Twilio → Whisper ASR → GPT-4 解析 → 中文通知 → 廚房
         ↑______確認與報價_________↓
```

### 技術棧
| 組件 | 成本/月 |
|------|---------|
| Twilio 號碼 | ~$25 |
| Whisper ASR | ~$10 |
| GPT-4 Parser | ~$15 |
| 微信企業號 | 免費 |
| **總計** | **~$50** |

## 📁 項目結構

```
├── dumpling_architecture.md    # 完整技術架構文檔
├── dumpling_dashboard.html     # 商業投影片 Dashboard
├── dumpling_presentation.html  # 快速演示版本
├── dumpling_modules/           # Python 源碼
│   ├── order_parser.py         # AI 訂單解析器
│   ├── twilio_handler.py       # Twilio 電話處理
│   ├── wechat_notifier.py      # 微信通知
│   └── kitchen_dashboard.html  # 廚房實時看板
└── index.html                  # 入口頁（本頁）
```

## 🚀 部署流程

本項目使用 **GitHub Actions** 自動部署到 GitHub Pages：

1. 推送代碼到 `main` 分支
2. Actions 自動觸發
3. 部署到 `https://你的用戶名.github.io/你的倉庫名/`

## 📅 實施計劃

### Phase 1: MVP (2週)
- ✅ Twilio 號碼申請
- ✅ 基礎訂單解析
- ✅ 微信通知測試

### Phase 2: 優化 (3週)
- 🔄 智能問答系統
- 🔄 訂單確認回撥
- 🔄 小票打印機整合

### Phase 3: 智能化 (4週)
- 🔴 Abacus POS 整合
- 🔴 預測等待時間
- 🔴 客戶畫像分析

## 📧 聯繫

項目由 OpenClaw AI Agent 自動生成。
