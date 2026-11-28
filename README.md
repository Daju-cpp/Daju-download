# 大橘桌面宠物 · 安装包下载

本仓库只托管**安装包**，源码不在公开区域。

## 许可

安装与使用前请阅读 [EULA.md](EULA.md)（最终用户许可协议 v1.0）。要点：

- 免费个人非商业使用，可原样完整转发安装包；
- 禁止反编译、拆包提取素材、改名换皮发布、二次售卖、去除作者标识；
- 商业使用需取得作者书面授权。

## 版本

| 版本 | 定位 | 说明 |
| --- | --- | --- |
| 主线版 | 完整功能 | 桌宠本体 + 内置浏览器 + AI 对话 + 邮箱 + 密码保险箱 |
| T 精简版 | 精简稳定 | 只保留桌宠本体，去掉浏览器 / AI / 保险箱 |

当前版本号：`v9.0 · build29.9`（主线）/ `v9.0 · build29.9T`（T 精简版）。

## 下载

全部安装包见 [Releases](https://github.com/Daju-cpp/Daju-download/releases)，无需登录：

| 文件 | 大小 | 说明 |
| --- | --- | --- |
| `DajuSetup_v9.0_build29.9.exe` | 241 MB | 主线版安装包（内置 WebView2 内核） |
| `DajuSetupT_v9.0_build29.9T.exe` | 4.0 MB | T 精简版安装包（无浏览器内核） |
| `Daju.exe` | 3.9 MB | 主线版可执行文件，免安装解压即用 |
| `SHA256SUMS.txt` | — | 上面三个文件的校验值，`sha256sum -c` 或 `certutil -hashfile` 核对 |

下载后建议核对校验值（Windows：`certutil -hashfile DajuSetup_v9.0_build29.9.exe SHA256`）：

```
b9bbc5fc429eeba75df6771c6774dc2faffdf924a2077060a71bfd7b0634a497  DajuSetup_v9.0_build29.9.exe
5c49ccf1140a2ff50df17d800e7c30658b3dfd69a4d0f294b7bbe51eacd3675a  DajuSetupT_v9.0_build29.9T.exe
1ce8f44b4668baa85720b86fc308e848dbf012130d39c31c2e46d46b717d52e7  Daju.exe
```

## 本版更新

- 邮箱模块：IMAP 检查 / 拉取列表 / 发信全部异步化，界面不再卡死；
- 支持 143 端口 STARTTLS，163 邮箱验证通过；
- 超时收紧：单次收发 12s、会话 45s、发信进程 30s，失败时按原因给出人话提示；
- 修复冷启动列表与提示文案不一致、状态行长文本被裁切两个问题。

## 关于

大橘是一个用 C++17 + Win32 写的 Windows 桌面萌宠，包含待机/走动/蹲坐/进食行为、番茄钟、待办提醒、便签、剪贴板历史、皮肤系统等本地功能。
