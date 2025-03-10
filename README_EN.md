# Web QQTang QQTPVE - WebAssembly Ported Version

<div align="center">
<img src="demo/demo.gif" alt="Demo of Web QQTang">

[Play in Browser](http://ikwbb.github.io/qqtpve)
</div><br>

**QQTPVE** is a highly faithful recreation of the classic game **QQTang**, originally developed by [atxxfs](https://github.com/atxxfs/QQTPVE). This project ports QQTPVE to the web using WebAssembly (WASM) technology, allowing players to experience this classic game directly in their browsers.

## Project Background

**QQTang** (QQT) is a classic casual competitive game developed by Tencent, beloved by many players. However, the official servers were shut down on **April 20, 2022**. **QQTPVE**, created by [atxxfs](https://github.com/atxxfs), is a near-perfect recreation of the original game’s gameplay and experience, making it one of the best QQTang revival projects to date. We extend our heartfelt thanks to the original author and all contributors!

This project aims to bring QQTPVE from the desktop to the web, making it more accessible for players to relive the fun of this classic game.

## Porting Details

### Technical Implementation
- **Original Code**: The original QQTPVE was written using **Pygame**.
- **Porting Tool**: [Pygbag](https://github.com/pmp-p/pygbag) was used to convert the game into WebAssembly (WASM) format for web execution.
- **Game Core**: Based on [detopoi/QQTPVE: By YongHeng ver20230418](https://github.com/detopoi/QQTPVE).
- **Resource Files**: Utilizes resources provided by [atxxfs](https://github.com/atxxfs).

### How to Play
1. Visit [the deployed webpage for this project](http://ikwbb.github.io/qqtpve).
2. Open it in a modern browser that supports WebAssembly (e.g., Chrome, Firefox).
3. Start playing and relive the classic QQTang experience!

## Current Issues

While the porting process is largely complete, some issues remain:
1. **Missing Game Resources**  
   - The current resources are primarily from the 2022 game version, missing some content available in the 2023 version.
   - We welcome community contributions of additional resource files to enhance the experience.
2. **Platform Compatibility**  
   - On devices like the iPad, `mixer.music` fails to play properly. A temporary workaround using `mixer.sound` is in place, but it may cause stuttering.
   - Future plans include optimizing audio playback for better compatibility and smoothness.

## Acknowledgments

- Thanks to [atxxfs](https://github.com/atxxfs) for developing such an outstanding QQTPVE recreation.
- Thanks to [detopoi](https://github.com/detopoi) for providing core code support.
- Thanks to all players and developers who have contributed to the QQTang community.

## How to Contribute

If you’re interested in this project, we welcome your participation in the following ways:
- Submit a Pull Request to help fix bugs or optimize the code.
- Provide missing game resources (e.g., assets from the 2023 version).
- Test the game and report issues (please submit an Issue).

## License

This project adheres to the license agreement of the original author [atxxfs](https://github.com/atxxfs/QQTPVE). The code for the WASM port follows the same license.
