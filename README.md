# Box-build

本仓库用于从 [xx025/Box](https://github.com/xx025/Box) 的 **main** 分支构建可安装的 APK，并发布到本仓库的 **Releases**。

## 下载 APK

- 打开 [Releases](https://github.com/xx025/Box-build/releases)
- 选择最新版本（按时间命名，格式：`v年.月.日.时分秒`，如 `v2026.02.16.144714`）
- 在页面底部下载对应架构的 APK

每次构建会产出 4 个 APK（arm64/armeabi × 通用/海信，均为 Normal Release、已签名）。

## 如何触发构建

1. 打开本仓库的 [Actions](https://github.com/xx025/Box-build/actions)
2. 左侧选择 **Build APK**
3. 点击 **Run workflow** → **Run workflow**

构建完成后会自动生成新的 Release 并上传 APK。

## 说明

- **源码**：[xx025/Box](https://github.com/xx025/Box)（fork 自 [takagen99/Box](https://github.com/takagen99/Box)）
- **构建分支**：`main`
- **签名**：使用与 [j4Uq/TVBoxOSC](https://github.com/j4Uq/TVBoxOSC) 相同的 Release 签名，便于安装与更新
