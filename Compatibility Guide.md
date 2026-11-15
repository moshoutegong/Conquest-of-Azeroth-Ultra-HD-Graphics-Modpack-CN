# 🧩 超高清补丁兼容与重命名指南

[返回简体中文首页](README.md) | [English](Compatibility%20Guide.en.md)

本指南适用于 **Conquest Reborn、ArdenWoW、Grimfall**，以及其他会检测修改过的客户端的自定义 WoW 3.3.5a 服务器。受 32 位客户端限制，使用过程中可能会遇到更多问题。

## 第一步：调整高清补丁文件名

进入游戏客户端的 `Data` 文件夹，按以下方式处理本整合包的补丁。

| 整合包文件 | 处理方式 |
| --- | --- |
| `patch-ZZB.MPQ` | 改名为 `patch-AAB.MPQ` |
| `patch-ZZE.MPQ` | 改名为 `patch-AAE.MPQ` |
| `patch-ZZD.MPQ` | 跳过本整合包里的这份文件。若已经复制进去，请移走这份高清文件 |

其他补丁可沿用原文件名。使用服务器原有的 **32 位客户端**启动游戏。

> [!NOTE]
> **汉化版补充。** 如果 Arden 客户端原本就有 `patch-ZZD.MPQ`，请保留原文件。上表只处理高清整合包提供的同名文件。

## 第二步：安装 32 位 LuxVelum

使用服务器原有的 32 位客户端时，请使用 [LuxVelum 的 Win32 发行版](https://github.com/Raz0r1337/LuxVelum/releases/tag/build-1)。按发布页说明将主包解压到游戏目录。若客户端没有内置 LuxVelum 加载功能，再安装该发布页提供的 Win32 `version.dll` 加载器。

**AMD 显卡用户**可在 `LuxVelum.ini` 中设置 `multisampling=0`。

## 第三步：配置其他增强内容

仍可使用包内的 ReShade 预设、`Config.wtf` 与额外插件。请根据自己的显示器调整 `Config.wtf` 中的分辨率和刷新率。

原指南让玩家把整合包 `x64` 文件夹中的 `d3d9.dll` 放到游戏根目录。

> [!IMPORTANT]
> **汉化版补充。** 先确认 DLL 的实际位数。此前核对过的整合包中，该 DLL 为 64 位。32 位 Arden 客户端需要匹配的 32 位 ReShade 组件。

## 兼容性声明

各服务器的补丁加载顺序可能不同，可能出现画面错误或其他问题。原作者按现状提供这些修改，其他服务器上的兼容问题不在其支持范围内。

本页根据 [fueryin 的英文兼容指南](https://github.com/fueryin/Conquest-of-Azeroth-Ultra-HD-Graphics-Modpack/blob/CoA-HD-PATCH/Compatibility%20Guide.md) 翻译。
