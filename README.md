# Price Currency Helper

See estimated conversions beside webpage prices, in a currency you choose.

**網頁換匯小幫手** — 保留原價，在辨識到的外幣價格旁顯示你選擇的貨幣估值。

[English](#english) · [繁體中文](#繁體中文) · [Privacy Policy / 隱私權政策](https://serpentvar.github.io/price-currency-helper/)

## English

### About

Price Currency Helper is a Chrome extension for comparing prices while browsing international websites. This repository hosts its public privacy policy and project information. Extension source code is not currently included here.

### Features

- Choose from 13 target currencies: **TWD, USD, JPY, EUR, GBP, HKD, KRW, CAD, AUD, SGD, CNY, THB and VND**.
- Keep original prices and add estimates beside recognized amounts.
- Recognize common currency symbols, codes, selected price ranges and dynamically updated prices.
- Use source-currency defaults for Taobao, Tmall, selected Amazon regional stores and Daytona Park, or set the source currency per website.
- Fetch and cache exchange-rate data locally, with manual overrides saved per source → target pair.
- Optionally add a fee percentage.
- Switch between English and Traditional Chinese, and enable or disable conversion globally or per website.
- Keep the bottom-right notification hidden during normal use; show it when a rate or connection problem occurs.

### Availability

The Chrome Web Store listing is being prepared. A verified store installation link will be added after publication.

### Privacy

Page text is processed locally to recognize prices. The extension does not upload page content, product prices or browsing URLs to the developer or exchange-rate provider.

Preferences, configured website domains, manual rates and cached exchange-rate tables are stored with `chrome.storage.local`. Exchange-rate requests go to ExchangeRate-API; the provider can receive ordinary connection information such as IP addresses. In v3.0.4, reading settings is local only. Disabled pages and pages whose detected currencies all have manual overrides do not trigger new automatic rate requests. Explicit Update rates clicks can still fetch rates; requests already sent are not retroactively cancelled.

There are no extension accounts, advertising SDKs, analytics trackers or telemetry in version 3.0.2.

Read the [full privacy policy](https://serpentvar.github.io/price-currency-helper/). The policy source is also available in [index.html](index.html).

### Limitations

Not every website or price format is supported. Prices in images, closed components, cross-origin iframes and browser-restricted pages may not work. Specify the source currency when `$` or `¥` is ambiguous or when you change a store's display currency.

Estimates do not separately calculate shipping, taxes, discounts or your payment provider's actual exchange costs. If the listed price includes tax, that listed amount is used for conversion. Checkout and your payment provider determine the final amount.

This is an independent project, not affiliated with Amazon, Taobao, Tmall or Daytona Park.

## 繁體中文

### 專案介紹

網頁換匯小幫手是一個方便瀏覽海外網站、比較標價的 Chrome 擴充功能。本儲存庫提供公開隱私權政策與專案說明，目前未包含擴充功能原始碼。

### 主要功能

- 提供 **13 種目標幣別**：台幣、美金、日圓、歐元、英鎊、港幣、韓元、加幣、澳幣、新加坡幣、人民幣、泰銖與越南盾。
- 保留原始標價，在辨識到的價格旁顯示估算金額。
- 支援常見貨幣符號、代碼、部分價格區間及動態更新的價格。
- 提供淘寶、天貓、部分 Amazon 地區站及 Daytona Park 的來源幣別預設，也能按網站指定幣別。
- 自動取得並快取匯率，手動匯率按「來源 → 目標」分開保存。
- 可選擇加計費用百分比。
- 提供繁體中文／英文介面、全域與單站開關。
- 右下角通知平常隱藏，匯率或連線有問題時才顯示。

### 安裝狀態

Chrome 線上應用程式商店資料準備中，正式發布後會補上經確認的安裝連結。

### 隱私

頁面文字只在本機用於辨識價格，不會把頁面內容、商品價格或瀏覽網址上傳給開發者或匯率服務。

偏好設定、指定網站網域、手動匯率與匯率快取保存在 `chrome.storage.local`。取得匯率時會連線至 ExchangeRate-API，服務方仍可收到 IP 等一般連線資訊。v3.0.4 讀取設定只在本機進行，停用頁面或頁面偵測到的幣別都有手動匯率時，不觸發新的自動匯率請求。主動按「更新匯率」仍可連線；已送出的請求不會追溯取消。

v3.0.2 沒有擴充功能帳號系統、廣告 SDK、分析追蹤或遙測。

詳見[完整隱私權政策](https://serpentvar.github.io/price-currency-helper/)，或檢視政策原始檔 [index.html](index.html)。

### 使用限制

不是所有網站或價格格式都能辨識。圖片價格、封閉元件、跨網域 iframe 及瀏覽器限制頁面可能不支援。當 `$`、`¥` 的幣別不明，或商店顯示幣別已變更，請自行指定來源幣別。

換算僅供參考，不會另外計算運費、稅金、折扣或付款機構的實際匯差。原始標價若含稅，就依該標價換算；實際付款以結帳與付款機構為準。

本專案與 Amazon、淘寶、天貓、Daytona Park 沒有隸屬或官方合作關係。

## Support / 聯絡方式

**Publisher / 發布者：Cassidy Chen**

Email: [cassidyvar@gmail.com](mailto:cassidyvar@gmail.com)

For a price-recognition issue, include the public page URL, the price location and a screenshot with personal details removed. Do not include passwords, payment details, order numbers or private account information.

回報價格辨識問題時，請附上公開商品網址、價格位置與移除個資後的截圖；不要提供密碼、付款資料、訂單編號或私人帳戶資訊。

## Exchange-rate attribution / 匯率來源

[Rates By Exchange Rate API](https://www.exchangerate-api.com) · [API documentation](https://www.exchangerate-api.com/docs/free)
