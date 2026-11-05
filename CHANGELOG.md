# Changelog

## 3.0.4 — 2026-11-05

- Process changed webpage regions in bounded batches instead of repeatedly rescanning the whole page.
- Validate finite numeric rates, base currency and source dates; reject malformed data and retain validated caches.
- Keep settings reads local. Suppress new automatic requests for disabled pages and fully manual conversion paths. Explicit popup refresh remains available.
- Preserve English and Traditional Chinese store metadata and existing price-detection support.
- Local fixture tests passed; real-site validation and Chrome Web Store review remain pending.

### 繁體中文

- 網頁掃描改為變更區塊、分批且限制工作量。
- 嚴格驗證匯率與日期，拒絕異常值並保留已驗證快取。
- 讀取設定不連網，停用頁面與全手動換算不新增自動取匯率請求；保留主動更新按鈕。
- 保留英／繁中商店語系與價格辨識功能。
- 本地模擬測試通過；真實網站實測與商店審查仍待完成。
