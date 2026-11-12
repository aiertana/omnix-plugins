# OilFX 油光/湿身效果

customoilfx（GameBanana mod 733773，Febby315 制作）的跟随更新与参数管理插件。

## 功能

- **一键安装 / 更新**：从 GameBanana 拉取 customoilfx 最新版，铺到 `WWMI\Mods` 根
- **参数调节**：强度滑条（0–2，写进 Matcap.ini）+ 风格化开关，游戏内按 Alt+0/± 键热调
- **按角色挂钩**：勾选角色生成 `OilFX@CharHooks.ini`（38 段内置挂钩，按角色过滤）
- **版本对比**：显示本地已装版本与 GameBanana 最新版本

## 下载

[OilFX-plugin.zip](./OilFX-plugin.zip)（约 76 MB，含 self-contained 独立界面，任何机器零依赖）

## 安装

OMniX → 功能专区 → 导入离线包 → 选这个 zip；或解压到 `GamesData\Plugins\OilFX\`。

## 界面来源（不同宿主版本）

| 宿主 | 界面 |
|------|------|
| 含 OilFXWindow 的新宿主 | 管道唤醒宿主窗口 |
| 其它版本 | **插件自带的独立 WinUI 界面**（与宿主同源 XAML，功能一致） |
| 极端兜底 | 精简版 WinForms 工具 |

## 版本历史

- **1.2.0**：新增独立 WinUI 界面（OilFXUI\，self-contained，旧版宿主也可用完整界面）；
  角色库头像（宿主 GamesData 优先，插件自带兜底）；启动器三级界面来源
- 1.1.x：宿主内置 OilFXWindow + 管道激活
- 1.0.0：初始版（启动器 + plugin.json）
