# !Mcode_ZHLocale · 中文界面驱动

![WoW 3.3.5a](https://img.shields.io/badge/WoW-3.3.5a-blue)

在 enUS 客户端上，让使用 AceLocale 机制且自带简体中文译文的插件显示中文。通过设置 `GAME_LOCALE = "zhCN"` 启用已有译文，缺失的翻译键回落英文。

这是一个界面语言驱动，不提供在线翻译，也不能让所有插件自动变成中文。

[下载源码 ZIP](https://github.com/MuyuQ/Mcode_ZHLocale/archive/refs/heads/main.zip) · [更新记录](CHANGELOG.md) · [反馈问题](https://github.com/MuyuQ/Mcode_ZHLocale/issues)

## 安装

1. 完全退出游戏，下载并解压 ZIP。
2. 将 TOC 所在文件夹改名为 **`!Mcode_ZHLocale`**，放入游戏的 `Interface/AddOns/`。
3. 重新启动游戏，在插件列表中启用本插件。

目录中应直接包含 `!Mcode_ZHLocale.toc` 和 `!Mcode_ZHLocale.lua`，不要多套一层目录。`!` 前缀用于提高加载优先级，请保留；实际加载顺序仍会受到其他插件依赖关系影响。

## 适用范围

- 目标客户端为魔兽世界 3.3.5a。
- 目标插件需要使用对应的 AceLocale 语言注册机制，并已经提供 `zhCN` 译文。
- 无中文词条、不使用该机制，或有额外语言守卫的插件，可能仍显示英文。
- 游戏任务、物品、地图、服务器文本与聊天翻译由各自资源或插件处理。

## 更新与停用

更新时备份并替换本插件目录，首次安装后完全重启。若覆盖整个 AddOns 目录后中文界面消失，检查驱动是否仍存在并启用。

在插件管理器或角色选择界面取消勾选，再 `/reload`，即可停止由本驱动设置语言。之后各插件使用自己的译文和配置；已安装的汉化资源及其他插件的中文不会因此撤销。

## 反馈

请提供目标插件名称、客户端版本，以及重载后仍显示英文的界面截图。部分插件没有自带中文译文，需要补充其译文，不能只靠语言驱动解决。

作者：Mcode。版本以 [`!Mcode_ZHLocale.toc`](!Mcode_ZHLocale.toc) 为准，历史变化见 [CHANGELOG](CHANGELOG.md)。
