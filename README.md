# Apple Silicon Compatibility List
Tracking the status of native Apple Silicon & Rosetta2-compatible builds of some popular **third-party** applications, tools and frameworks.

Data is collected from the internet, as I have no Apple Silicon hardware yet to confirm the status (a Mac Mini is on its way).

If you encounter any errors or if you'd like to add your favorite app/framework to the list, please open an issue or submit a pull request. Thanks!

**Last update**: *Nov 13th 2020*

#### Status Legend
* ✅ Native Apple Silicon build exists, public download available
* ✓ Native build exists, but not confirmed yet
* 💎 No native build, but working under Rosetta2
* ⛔️ No native build, not working under Rosetta2
* 🔄 No native build, unknown if build works under Rosetta2

## Table of contents

  - [Browser](#Browser) | [Communication](#Communication) | [Graphics](#Graphics) | [Video](#Video) | [Audio](#Audio) | [Utilities](#Utilities)
  - [Developer](#Developer) | [Virtualization](#Virtualization) | [Frameworks](#Frameworks) | [Languages](#Languages)

### Browser

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Chrome|🔄|||Depends on Chromium, see [Frameworks](#Frameworks)|
|Brave|🔄|||Depends on Chromium, see [Frameworks](#Frameworks)|
|Firefox|🔄||[[meta] Support AArch64 on Desktop macOS (Apple Silicon)](https://bugzilla.mozilla.org/show_bug.cgi?id=1648496)||

### Communication

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Skype|🔄||||
|Whatsapp|🔄|||Depends on Electron, see [Frameworks](#Frameworks)|
|Microsoft Office 2019|✅|2019 Beta||Available in the [Beta Channel](https://insider.office.com/en-us/join/mac) only|

### Graphics

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Sketch|🔄||||
|[Pixelmator Pro](https://www.pixelmator.com/pro/)|✅|2.0+||Will be available 11/19/2020|
|Adobe Photoshop|🔄|||||

### Video

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|FFmpeg|✓|4.3.1||Builds according to [this report](http://www.ffmpeg-archive.org/FFmpeg-on-Apple-Silicon-Success-td4693516.html), but no binary builds available yet.|
|[Handbrake](https://github.com/HandBrake/HandBrake/releases)|✅|1.4.0+|||
|VLC|🔄||||

### Audio

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Spotify|🔄|||Depends on Electron, see [Frameworks](#Frameworks)|

### Utilities

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Arq Backup|🔄|||||
|KeepassXC|🔄||||
|Bear|🔄||||
|Notability|🔄||||
|Kindle|🔄||||
|WireGuard|🔄||||

### Developer

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|VS Code|🔄||[Stablize apple silicon exploration builds #106770](https://github.com/microsoft/vscode/issues/106770)||
|[Tower](https://www.git-tower.com/download/mac)|✅|6.0+||https://www.git-tower.com/blog/tower-mac-6|
|Insomnia|🔄|||Depends on Electron, see [Frameworks](#Frameworks)|
|Homebrew|🔄||Status of all the core formulae: [macOS 11.0 Big Sur compatibility on Apple Silicon #7857](https://github.com/Homebrew/brew/issues/7857)||

### Virtualization

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Parallels Desktop|✓|Technical Preview||[Parallels Desktop for Mac with Apple M1 chip](https://www.parallels.com/blogs/parallels-desktop-apple-silicon-mac/)|
|Docker|⛔️||[Docker fails to launch on Apple Silicon #4733](https://github.com/docker/for-mac/issues/4733)||

### Frameworks

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Qt|⛔️||[Qt for macOS on Apple Silicon (arm64)](https://bugreports.qt.io/browse/QTBUG-85279)||
|Electron|✓|11.0.0-beta.1|[Apple Silicon / macOS Big Sur Support #24319](https://github.com/electron/electron/issues/24319)|[Electron Blog: Apple Silicon Support](https://www.electronjs.org/blog/apple-silicon)|
|Chromium|✅||<ul><li>[Building Chromium on ARM64](https://bugs.chromium.org/p/chromium/issues/detail?id=1103236)</li><li>[Building Chromium for ARM64 (Intel host)](https://bugs.chromium.org/p/chromium/issues/detail?id=1098899)</li><li>[All related Chromium issues](https://bugs.chromium.org/p/chromium/issues/list?q=label%3AMac-BigSur%20OR%20label%3AMac-Arm64&can=2)</li></ul>|You can now [build an universal binary on an Intel Mac](https://chromium.googlesource.com/chromium/src.git/+/master/docs/mac_arm64.md)|


### Languages

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Python|✓|3.8|[add support for macos 11.0, arm64, universal2 #319](https://github.com/pypa/packaging/pull/319)||
|Rust|⛔️||[Tracking issue for supporting macOS on Apple Silicon (ARM) #73908](https://github.com/rust-lang/rust/issues/73908)||
|R|⛔️|||[Will R Work on Apple Silicon?](https://developer.r-project.org/Blog/public/2020/11/02/will-r-work-on-apple-silicon/index.html)|

