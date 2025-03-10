# QQT堂網頁版 QQTPVE - WebAssembly 移植版

<div align="center">
<img src="demo/demo.gif" alt="Demo of Web QQTang">

[在线试玩](http://ikwbb.github.io/qqtpve)
     
</div><br>

**QQTPVE** 是一個基於經典遊戲 **QQ堂** 的高度復刻版本，原作者為 [atxxfs](https://github.com/atxxfs/QQTPVE)。本項目將 QQTPVE 移植到網頁端，通過 WebAssembly (WASM) 技術，讓玩家能夠直接在瀏覽器中體驗這款經典遊戲。

## 項目背景

**QQ堂**（QQTang）是一款由騰訊開發的經典休閒競技遊戲，深受玩家喜愛。然而，官方服務器已於 **2022年4月20日** 正式關閉。**QQTPVE** 是由 [atxxfs](https://github.com/atxxfs) 開發的復刻版本，幾乎完美還原了原版遊戲的玩法和體驗，是目前最出色的 QQ堂 復刻項目之一。在此向原作者及相關貢獻者致以誠摯的感謝！

本項目旨在將 QQTPVE 從桌面端移植到網頁端，讓更多玩家能夠便捷地重溫這款遊戲的樂趣。

## 移植說明

### 技術實現
- **原始代碼**：QQTPVE 原版由 **Pygame** 編寫。
- **移植工具**：使用 [Pygbag](https://github.com/pmp-p/pygbag) 將遊戲轉換為 WebAssembly (WASM) 格式，從而實現網頁端的運行。
- **遊戲核心**：基於 [detopoi/QQTPVE: By YongHeng ver20230418](https://github.com/detopoi/QQTPVE) 的版本。
- **資源文件**：使用 [atxxfs](https://github.com/atxxfs) 提供的 Resources。

### 如何遊玩
1. 訪問![本項目部署的網頁鏈接](http://ikwbb.github.io/qqtpve)。
2. 在支持 WebAssembly 的現代瀏覽器中直接打開（推薦 Chrome、Firefox 等）。
3. 開始遊戲，重溫 QQ堂 的經典體驗！

## 目前存在的問題

儘管移植已經基本完成，但仍有一些待解決的問題：
1. **遊戲資源缺失**  
   - 當前資源主要來自 2022 年的遊戲版本，相比 2023 年版本缺少部分內容。
   - 歡迎社區貢獻更多資源文件以完善遊戲體驗。
2. **平臺兼容性**  
   - 在 iPad 等設備上，`mixer.music` 無法正常播放，目前臨時使用 `mixer.sound` 替代，但可能導致卡頓。
   - 未來計劃優化音頻播放的兼容性和流暢性。

## 致謝

- 感謝 [atxxfs](https://github.com/atxxfs) 開發了如此出色的 QQTPVE 復刻版本。
- 感謝 [detopoi](https://github.com/detopoi) 提供的核心代碼支持。
- 感謝所有為 QQ堂 社區做出貢獻的玩家和開發者。

## 如何貢獻

如果你對本項目感興趣，歡迎參與以下內容：
- 提交 Pull Request，幫助修復 Bug 或優化代碼。
- 提供缺失的遊戲資源（如 2023 年版本的素材）。
- 測試遊戲並反饋問題（請提交 Issue）。


## 許可協議

本項目遵循原作者 [atxxfs](https://github.com/atxxfs/QQTPVE) 的許可協議。WASM 移植部分的代碼同樣遵循相同協議。
