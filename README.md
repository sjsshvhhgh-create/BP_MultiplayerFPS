# 🎮 BP_MultiplayerFPS - 局域网联机抢怪射击手游

基于 **Unreal Engine 5 (虚幻引擎5)** 纯蓝图打造的移动端多人第一人称射击（FPS）竞技游戏。本项目已完美打通安卓真机编译与部署链，支持双机 WiFi 局域网实时同步联机对战。

---

## ✨ 核心核心机制与功能

* **⚡ 局域网联机底层**：基于虚幻引擎网络架构，实现非专用服务器（Listen Server）的双机 WiFi 局域网秒级寻路与加入。
* **⚔️ 多人蓝图同步**：完美打通射击弹道、怪物生成、开枪销毁等核心逻辑的 Server/Client 双向同步。
* **📊 实时计分系统**：全新的手搓功能 UI 界面，支持抢怪击杀实时全网弹框算分。
* **🏆 胜利结算定格**：率先抢怪达到 **10 分** 满分的玩家触发全屏获胜特效，游戏定格收网。

---

## 📲 快速开始 / 玩家体验

如果你只想直接在手机上体验游戏，请前往本仓库右侧的 [Releases (发行版)](https://github.com/sjsshvhhgh-create/BP_MultiplayerFPS/releases) 页面：

1.  下载 **`BP_MultiplayerFPS-arm64.apk`** 并安装至您的安卓手机（支持 Android 8.0 及以上）。
2.  确保两台手机连接在 **同一个 WiFi 局域网** 下。
3.  **手机 A (房主)**：点击 UI 上的 **`Host`** 按钮建立房间。
4.  **手机 B (客机)**：查看手机 A 的局域网 IP（如 `192.168.1.X`），在输入框输入该 IP 后点击 **`Join`** 即可合流开战！
5.  *（可选）* 可下载 Release 页面下的 `Gameplay.mp4` 观看实况联机演示。

---

## 🛠️ 开发者本地部署与编译环境

如果你想下载本仓库源码并在本地进行二次开发或打包，请确保您的虚幻引擎安卓环境完全对齐以下标准（历经版本冲突实战验证的最稳配置）：

* **引擎版本**：Unreal Engine 5.x
* **Android SDK / NDK**：
    * Minimum SDK: `26` (Android 8.0)
    * Target SDK: `33` (Android 13)
* **编译工具链**：
    * **Gradle**: `7.5`
    * **JDK (Java)**: `17` 或 `21`（已彻底修复包名带中括号及多版本代差引起的编译死锁）

### 📥 本地克隆源码：
```bash
git clone [https://github.com/sjsshvhhgh-create/BP_MultiplayerFPS.git](https://github.com/sjsshvhhgh-create/BP_MultiplayerFPS.git)
