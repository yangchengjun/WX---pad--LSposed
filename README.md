# HideDeviceLoginTip

一个 LSPosed/Xposed 模块，用于隐藏微信和 QQ 的设备登录状态栏提示。

## 功能说明

| 应用 | 隐藏内容 |
|------|----------|
| 微信 | "1个设备已登录微信"、"平板微信已登录"、"Windows微信已登录" 等 |
| QQ | "已登录 Pad"、"已登录 Windows"、"已登录 Windows、Pad" 等 |

**注意**：本模块只隐藏 UI 显示，**不会阻止**扫码登录其他设备的功能。

## 下载

| 版本 | 下载 | 更新日期 |
|------|------|----------|
| v1.0.0 | [WQ_hid_v1.0.0.apk](WQ_hid_v1.0.0.apk) | 2026-01-11 |

## 安装使用

### 环境要求
- Android 9.0+ (API 28+)
- LSPosed 或其他 Xposed 框架
- 微信 / QQ 应用

### 安装步骤
1. 下载 APK 并安装
2. 在 LSPosed 管理器中启用模块
3. 勾选作用域：
   - 微信 (com.tencent.mm)
   - QQ (com.tencent.mobileqq)
4. 打开模块设置界面，按需开启/关闭各应用的屏蔽功能
5. 强制停止并重新打开微信/QQ

## 截图

<待添加>

## 常见问题

### Q: 状态栏有时会短暂出现？
A: 这是正常现象，模块会在几十毫秒内将其隐藏。

### Q: 修改设置后没有生效？
A: 需要强制停止并重新打开目标应用。

### Q: 会影响扫码登录功能吗？
A: 不会。本模块只隐藏 UI 显示，不影响任何登录功能。

## 技术栈

- YukiHookAPI
- DexKit
- Kotlin

## 免责声明

本项目仅供学习交流使用。使用本模块可能违反相关应用的用户协议，请自行承担风险。

## 致谢

- [YukiHookAPI](https://github.com/HighCapable/YukiHookAPI)
- [DexKit](https://github.com/LuckyPray/DexKit)
- [LSPosed](https://github.com/LSPosed/LSPosed)

## License

本项目采用 [MIT License](LICENSE) 开源协议发布。
