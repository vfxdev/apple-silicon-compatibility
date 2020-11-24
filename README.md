# Apple Silicon Compatibility List
Tracking the status of native Apple Silicon & Rosetta2-compatible builds of some popular **third-party** applications, tools and frameworks.

~~Data is collected from the internet, as I have no Apple Silicon hardware yet to confirm the status (a Mac Mini is on its way).~~ My Mac Mini has arrived and I've started to add first-hand confirmations to the list.

If you encounter any errors or if you'd like to add your favorite app/framework to the list, please open an issue or submit a pull request. Thanks!

**Last update**: *Nov 24th 2020*

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
|[Chrome](https://www.google.com/chrome/)/Chromium|✅|87|[Building Chromium on ARM64](https://bugs.chromium.org/p/chromium/issues/detail?id=1103236)<br>[Building Chromium for ARM64 (Intel host)](https://bugs.chromium.org/p/chromium/issues/detail?id=1098899)<br>[All related Chromium issues](https://bugs.chromium.org/p/chromium/issues/list?q=label%3AMac-BigSur%20OR%20label%3AMac-Arm64&can=2)||
|Brave|💎||[arm64 support for macOS (Apple Silicon, M1 CPU) #12819](https://github.com/brave/brave-browser/issues/12819)|Depends on Chromium|
|Firefox|✅|Nightly|[[meta] Support AArch64 on Desktop macOS (Apple Silicon)](https://bugzilla.mozilla.org/show_bug.cgi?id=1648496)|Nightly build is now a universal binary according to [this tweet](https://twitter.com/gcpascutto/status/1327153863598755840).|

### Communication

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Skype|💎|||Depends on Electron, see [Frameworks](#Frameworks)|
|Whatsapp|💎|||Depends on Electron, see [Frameworks](#Frameworks)|
|Discord|💎|||Depends on Electron, see [Frameworks](#Frameworks)|
|Telegram|💎|||Native MacOS client, should work with Rosetta2, but unconfirmed|
|Microsoft Office 2019|✅|2019 Beta||Available in the [Beta Channel](https://insider.office.com/en-us/join/mac) only|

### Graphics

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|[Sketch](https://www.sketch.com/beta/)|✅|70 beta+||69 and earlier work on Rosetta2|
|[Pixelmator Pro](https://www.pixelmator.com/pro/)|✅|2.0+||Will be available 11/19/2020|
|[Affinity Photo/Designer/Publisher](https://affinity.serif.com/en-us/)|✅|1.8.6+||[Blog post](https://affinity.serif.com/en-us/apple-m1-chip-support/)|
|[Adobe Photoshop](https://feedback.photoshop.com/conversations/photoshop-beta/photoshop-for-mac-arm-is-here/5fb359d3ca9d527a59c4677e)|✅|ARM Beta|[Known Issues under Rosetta2](https://helpx.adobe.com/photoshop/kb/photoshop-and-macos-big-sur.html)|Native beta released 11/17/2020|
|Adobe Lightroom|💎|4.x||Native support expected December 2020, according to [Lightroom and Big Sur](https://helpx.adobe.com/lightroom-cc/kb/macos-big-sur-compatibility.html)|
|Adobe Lightroom Classic|💎|11.x||Native support expected 2021, according to [Lightroom Classic and Big Sur](https://helpx.adobe.com/lightroom-classic/kb/macos-big-sur-compatibility.html)|
|Blender|🔄||[macOS: Support arm64](https://developer.blender.org/T78710)||


### Video

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|[DaVinci Resolve](https://www.blackmagicdesign.com/products/davinciresolve/)|✅|17.1 Beta 1|||
|FFmpeg|✓|4.3.1||Builds according to [this report](http://www.ffmpeg-archive.org/FFmpeg-on-Apple-Silicon-Success-td4693516.html), but no binary builds available yet.|
|[Handbrake](https://github.com/HandBrake/HandBrake/releases)|✅|1.4.0+|||
|VLC|🔄||||

### Audio

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Spotify|💎|||Depends on Electron, see [Frameworks](#Frameworks)|

### Utilities

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|1Password|💎|||Works under Rosetta2 according to [Will 1password run on Apple silicon-based Mac](https://1password.community/discussion/114181/will-1password-run-on-apple-silicon-based-mac)|
|[Alfred](https://www.alfredapp.com/universal/)|✅|4.2.1.b1186+||||
|[Arq Backup](https://www.arqbackup.com/download/)|💎|5.x, 7.x||Both versions work under Rosetta2, according to developer.|
|Bear|✅|1.8.2|||
|KeepassXC|💎|||Depends on Qt, see [Frameworks](#Frameworks)|
|Kindle|💎|||via App Store|
|Notability|💎|||via App Store|
|WireGuard|💎||||

### Developer

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|[VS Code](https://code.visualstudio.com/insiders/)|✅||[Stablize apple silicon exploration builds #106770](https://github.com/microsoft/vscode/issues/106770)|Exploration build linked in issue works great.|
|[Tower](https://www.git-tower.com/download/mac)|✅|6.0+||https://www.git-tower.com/blog/tower-mac-6, make sure you have Rosetta2 installed, otherwise it will crash.|
|Insomnia|💎|2020.4.2||Depends on Electron, see [Frameworks](#Frameworks)|
|[iTerm2](https://iterm2.com/downloads.html)|✅|3.4.0+|||
|Homebrew|⛔️||Status of all the core formulae: [macOS 11.0 Big Sur compatibility on Apple Silicon #7857](https://github.com/Homebrew/brew/issues/7857)|Most of it works, but still lot of formulae are failing. Will not be fully compatible for months, according to devs.|
|Unity Player|✅|2020.2.0a21+|Status of all the core formulae: [Unity on Apple silicon and Big Sur: Known issues and workarounds](https://forum.unity.com/threads/unity-on-apple-silicon-and-big-sur-known-issues-and-workarounds.929220/)||
|Unity Editor|💎|2020.2.0b12+|see Unity Player||

2020.2.0a21

### Virtualization

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Parallels Desktop|✓|Technical Preview||[Parallels Desktop for Mac with Apple M1 chip](https://www.parallels.com/blogs/parallels-desktop-apple-silicon-mac/)|
|Docker|⛔️||[Docker fails to launch on Apple Silicon #4733](https://github.com/docker/for-mac/issues/4733)|[Apple Silicon M1 Chips and Docker](https://www.docker.com/blog/apple-silicon-m1-chips-and-docker/?utm_campaign=IT+Pro&utm_content=1605547520&utm_medium=social&utm_source=Organic). Depends on Electron and Go, see [Frameworks](#Frameworks)|

### Frameworks

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Qt|⛔️||[Qt for macOS on Apple Silicon (arm64)](https://bugreports.qt.io/browse/QTBUG-85279)<br>[Qt issues on Rosetta2](https://bugreports.qt.io/browse/QTBUG-86405)|QtWebEngine [doesn't work on Rosetta2](https://bugreports.qt.io/browse/QTBUG-86406) due to dependency on Chromium. A [developer reports](https://bugreports.qt.io/browse/QTBUG-85279?focusedCommentId=529211&page=com.atlassian.jira.plugin.system.issuetabpanels:comment-tabpanel#comment-529211) successful native ARM build of Qt 5.12.7 by applying latest patches.|
|Electron|✅|11.0|[Apple Silicon / macOS Big Sur Support #24319](https://github.com/electron/electron/issues/24319)|[Electron Blog: Apple Silicon Support](https://www.electronjs.org/blog/apple-silicon)|

### Languages

|Name|Status|Version|Issues|Notes|
|--|:---:|--|--|--|
|Python|✅|3.8+|[Support macOS 11 and Apple Silicon #22855](https://github.com/python/cpython/pull/22855)|3.9 is also native via Homebrew|
|Go|⛔️||[runtime: tracking bug for ARM-based macOS and GOOS/GOARCH values #38485](https://github.com/golang/go/issues/38485)||
|Rust|⛔️||[Tracking issue for supporting macOS on Apple Silicon (ARM) #73908](https://github.com/rust-lang/rust/issues/73908)||
|R|⛔️|||[Will R Work on Apple Silicon?](https://developer.r-project.org/Blog/public/2020/11/02/will-r-work-on-apple-silicon/index.html)|

