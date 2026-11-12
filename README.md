# OMniX 插件库

OMniX 功能专区插件的集中仓库。**每个插件一个独立目录，按需分别下载对应的 zip 离线包即可**。

## 插件索引

| 插件 | 版本 | 功能 | 宿主要求 | 下载 |
|------|------|------|----------|------|
| [OilFX 油光/湿身效果](./OilFX/) | 1.2.0 | customoilfx（mod 733773）跟随更新 + 参数调节 + 按角色挂钩 | 全版本（新宿主直开，旧版本自动用内置界面） | [OilFX-plugin.zip](./OilFX/OilFX-plugin.zip) |
| [GameBanana](./GameBananaStore/) | 1.1.0 | GameBanana 在线商店：浏览/搜索/下载/安装 mod | v1.4.6+ 管道秒开；v1.4.5 自动 UIA 兜底 | [GameBananaStore-plugin.zip](./GameBananaStore/GameBananaStore-plugin.zip)（源码仓库：[OMniX-GameBanana](https://github.com/aiertana/OMniX-GameBanana)） |

## 安装方法

**方式一（推荐）：功能专区导入**

OMniX → 功能专区 → 「导入离线包」→ 选择对应插件的 zip → 卡片出现。

**方式二：手动解压**

把 zip 解压到 OMniX 的 `GamesData\Plugins\<插件名>\` 目录（zip 内已有同名目录），重启 OMniX。

## 版本对应表

| OMniX 宿主 | OilFX 行为 | GameBanana 行为 |
|-----------|-----------|----------------|
| v1.4.7+（含 OilFXWindow） | 管道唤醒宿主界面（同源 XAML） | 管道直开商店 |
| v1.4.6 | 独立 WinUI 界面（插件自带，与宿主同源） | 管道直开商店 |
| v1.4.5（无管道） | 独立 WinUI 界面 | UIA 自动化兜底 |
| 更旧版本 | 独立 WinUI 界面 / 精简工具兜底 | UIA 自动化兜底 |

> 插件对旧版本宿主的适配原理：插件自带完整管理界面（OilFX 为 self-contained
> WinUI 应用，运行时全打包，目标机器零依赖），宿主只负责「点卡片拉起插件」。

## 目录结构

```
omnix-plugins/
├── OilFX/                     # OilFX 插件（离线包 + 说明）
│   ├── README.md
│   ├── plugin.json
│   └── OilFX-plugin.zip
└── GameBananaStore/           # GameBanana 商店插件
    ├── README.md
    ├── plugin.json
    └── GameBananaStore-plugin.zip
```

> zip 用 ASCII 文件名：OMniX 功能专区的「下载插件」按钮直接拉
> `raw.githubusercontent.com/aiertana/omnix-plugins/main/<目录>/<文件>.zip`，
> 免得中文文件名的 URL 编码出幺蛾子。

## 许可

各插件 LICENSE 见其源码仓库（均为 MIT）。
