<div align="center">

# QQT堂网页版 QQTPVE - WebAssembly 移植版

     
<img src="demo/demo.gif" alt="Demo of Web QQTang">

[在线试玩](http://ikwbb.github.io/qqtpve)

[简体中文](#) | [繁体中文](README_HK.md) | [English](README_EN.md)


</div><br>


**QQTPVE** 是一个基于经典游戏 **QQ堂** 的高度复刻版本，原作者为 [atxxfs](https://github.com/atxxfs/QQTPVE)。本项目将 QQTPVE 移植到网页端，通过 WebAssembly (WASM) 技术，让玩家能够直接在浏览器中体验这款经典游戏。

## 项目背景

**QQ堂**（QQTang）是一款由腾讯开发的经典休闲竞技游戏，深受玩家喜爱。然而，官方服务器已于 **2022年4月20日** 正式关闭。**QQTPVE** 是由 [atxxfs](https://github.com/atxxfs) 开发的复刻版本，几乎完美还原了原版游戏的玩法和体验，是目前最出色的 QQ堂 复刻项目之一。在此向原作者及相关贡献者致以诚挚的感谢！

本项目旨在将 QQTPVE 从桌面端移植到网页端，让更多玩家能够便捷地重温这款游戏的乐趣。


### 如何游玩
1. 访问[本项目部署的网页链接](http://ikwbb.github.io/qqtpve)。
2. 在支持 WebAssembly 的现代浏览器中直接打开（推荐 Chrome、Firefox 等）。
3. 开始游戏，重温 QQ堂 的经典体验！


## 移植说明

### 技术实现
- **原始代码**：QQTPVE 原版由 **Pygame** 编写。
- **移植工具**：使用 [Pygbag](https://github.com/pmp-p/pygbag) 将游戏转换为 WebAssembly (WASM) 格式，从而实现网页端的运行。
- **游戏核心**：基于 [detopoi/QQTPVE: By YongHeng ver20230418](https://github.com/detopoi/QQTPVE) 的版本。
- **资源文件**：使用 [atxxfs](https://github.com/atxxfs) 提供的 Resources。


## 目前存在的问题

尽管移植已经基本完成，但仍有一些待解决的问题：
1. **游戏资源缺失**  
   - 当前资源主要来自 2022 年的游戏版本，相比 2023 年版本缺少部分内容。
   - 欢迎社区贡献更多资源文件以完善游戏体验。
2. **平台兼容性**  
   - 在 iPad 等设备上，`mixer.music` 无法正常播放，目前临时使用 `mixer.sound` 替代，但可能导致卡顿。
   - 未来计划优化音频播放的兼容性和流畅性。

## 致谢

- 感谢 [atxxfs](https://github.com/atxxfs) 开发了如此出色的 QQTPVE 复刻版本。
- 感谢 [detopoi](https://github.com/detopoi) 提供的核心代码支持。
- 感谢所有为 QQ堂 社区做出贡献的玩家和开发者。

## 如何贡献

如果你对本项目感兴趣，欢迎参与以下内容：
- 提交 Pull Request，帮助修复 Bug 或优化代码。
- 提供缺失的游戏资源（如 2023 年版本的素材）。
- 测试游戏并反馈问题（请提交 Issue）。

## 许可协议

本项目遵循原作者 [atxxfs](https://github.com/atxxfs/QQTPVE) 的许可协议。WASM 移植部分的代码同样遵循相同协议。
