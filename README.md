# Apple Silicon Compatibility List
Tracking the status of native Apple Silicon & Rosetta2-compatible builds of some popular **third-party** applications, tools and frameworks.

Data is collected from the internet, as I have no Apple Silicon hardware yet to confirm the status (a Mac Mini is on its way).

If you encounter any errors or if you'd like to add your favorite app/framework to the list, please open an issue or submit a pull request. Thanks!

**Last update**: *Nov 13th 2020*

#### Status Legend
* ✅ Works, confirmed, public download available
* ✓ Works, but unconfirmed
* ⛔️ Not working
* 🔄 Unknown

## Table of contents

  - [🕸 Browser](#-browser) | [📡 Communication](#-communication) | [🎨 Graphics](#-graphics) | [🎬 Video](#-video) | [🔈 Audio](#-audio) | [🛠 Utilities](#-utilities)
  - [💻 Developer](#-developer-apps) [🥞 Virtualization](#-virtualization) [🧩 Frameworks](#-frameworks) [🗣 Languages](#-languages)

### 🕸 Browser
|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|Chrome|⛔️|🔄|||Depends on Chromium, see [🧩 Frameworks](#-frameworks)|
|Brave|⛔️|🔄|||Depends on Chromium, see [🧩 Frameworks](#-frameworks)|
|Firefox|⛔️|🔄||[[meta] Support AArch64 on Desktop macOS (Apple Silicon)](https://bugzilla.mozilla.org/show_bug.cgi?id=1648496)||

### 📡 Communication

|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|Skype|⛔️|🔄||||
|Whatsapp|⛔️|🔄|||Depends on Electron, see [🧩 Frameworks](#-frameworks)|

### 🎨 Graphics
|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|Sketch|⛔️|🔄||||
|Pixelmator Pro|⛔️|✓||||
|Adobe Photoshop|⛔️|✓||||

### 🎬 Video
|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|FFmpeg|✓|🔄|4.3.1||Builds according to [this report](http://www.ffmpeg-archive.org/FFmpeg-on-Apple-Silicon-Success-td4693516.html), but no binary builds available yet.|
|VLC|⛔️|🔄||||

### 🔈 Audio
|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|Spotify|⛔️|🔄|||Depends on Electron, see [🧩 Frameworks](#-frameworks)|

### 🛠 Utilities
|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|Arq Backup|⛔️|🔄|||||
|KeepassXC|⛔️|🔄||||
|Bear|⛔️|🔄||||
|Notability|⛔️|🔄||||
|Kindle|⛔️|🔄||||
|WireGuard|⛔️|🔄||||

### 💻 Developer
|Name|Native|Rosetta2|Version|Issues|Notes|
|--|--|--|--|--|--|
|VS Code|⛔️|🔄||[Stablize apple silicon exploration builds #106770](https://github.com/microsoft/vscode/issues/106770)||
|Tower|✓|🔄|6.0||https://www.git-tower.com/blog/tower-mac-6|
|Insomnia|⛔️|🔄|||Depends on Electron|
|Homebrew|⛔️|🔄||Status of all the core formulae: [macOS 11.0 Big Sur compatibility on Apple Silicon #7857](https://github.com/Homebrew/brew/issues/7857)||
### 🥞 Virtualization
|Name|Native|Version|Issues|Notes|
|--|--|--|--|--|
|Parallels Desktop|✓|Technical Preview||[Parallels Desktop for Mac with Apple M1 chip](https://www.parallels.com/blogs/parallels-desktop-apple-silicon-mac/)|
|Docker|⛔️||[Docker fails to launch on Apple Silicon #4733](https://github.com/docker/for-mac/issues/4733)||

### 🧩 Frameworks
|Name|Native|Version|Issues|Notes|
|--|--|--|--|--|
|Qt|⛔️||[Qt for macOS on Apple Silicon (arm64)](https://bugreports.qt.io/browse/QTBUG-85279)||
|Electron|✓|11.0.0-beta.1|[Apple Silicon / macOS Big Sur Support #24319](https://github.com/electron/electron/issues/24319)|[Electron Blog: Apple Silicon Support](https://www.electronjs.org/blog/apple-silicon)|
|Chromium|⛔️||<ul><li>[Building Chromium on ARM64](https://bugs.chromium.org/p/chromium/issues/detail?id=1103236)</li><li>[Building Chromium for ARM64 (Intel host)](https://bugs.chromium.org/p/chromium/issues/detail?id=1098899)</li><li>[All related Chromium issues](https://bugs.chromium.org/p/chromium/issues/list?q=label%3AMac-BigSur%20OR%20label%3AMac-Arm64&can=2)</li></ul>||


### 🗣 Languages
|Name|Native|Version|Issues|Notes|
|--|--|--|--|--|
|Python|✓|3.8|[add support for macos 11.0, arm64, universal2 #319](https://github.com/pypa/packaging/pull/319)||
|Rust|⛔️||[Tracking issue for supporting macOS on Apple Silicon (ARM) #73908](https://github.com/rust-lang/rust/issues/73908)||
|R|⛔️|||[Will R Work on Apple Silicon?](https://developer.r-project.org/Blog/public/2020/11/02/will-r-work-on-apple-silicon/index.html)|

