p>

<h1 align="center">My_Capture 9.3</h1>

<p align="center">
  A Windows screenshot tool with whole-window and internal-region detection, accurate rounded corners, system tray integration, startup launch, and multilingual UI.<br>
  一款面向 Windows 的截图工具，支持整窗与窗口内部区域识别、真实圆角、系统托盘、开机启动和多语言界面。<br>
  ウィンドウ全体・内部領域の検出、正確な角丸、システムトレイ、自動起動、多言語 UI に対応した Windows 向けスクリーンショットツール。
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Windows%2010%20%7C%2011-0078D4" alt="Windows">
  <img src="https://img.shields.io/badge/Distribution-Binary%20Release-555555" alt="Binary Release">
  <img src="https://img.shields.io/badge/Version-9.3-blue" alt="Version">
  <img src="https://img.shields.io/badge/Source%20Code-Not%20Published-lightgrey" alt="Source Code Not Published">
</p>

<p align="center">
  <a href="#简体中文">简体中文</a> ·
  <a href="#english">English</a> ·
  <a href="#日本語">日本語</a>
</p>

---

## Preview / 软件预览 / プレビュー

> 将软件截图放到下面路径后，GitHub 会自动显示。  
> Place screenshots in the following paths.  
> 次のパスにスクリーンショットを配置してください。

### Main window / 主界面 / メイン画面

<img width="1008" height="789" alt="2026-07-11_15-15-01" src="https://github.com/user-attachments/assets/4df94741-1319-4422-ae51-e93588e28cb0" />





---

# 简体中文

## 作品介绍

**My_Capture 9.3** 是一款面向 Windows 10 和 Windows 11 的桌面截图工具。

它不仅支持常规的手动区域截图、窗口截图和全屏截图，还能识别窗口内部的标题栏、工具栏、地址栏、侧边栏、内容区和状态栏。软件对 Windows 圆角窗口进行了专门处理，并提供图库、底部图片信息栏、系统托盘、开机启动、快捷键、自定义图标和多语言界面。

本仓库用于：

- 发布软件成品
- 提供版本更新说明
- 展示软件截图
- 提供 Windows EXE 下载
- 收集 Bug 反馈和功能建议

本项目**不公开源代码**。GitHub Releases 中提供的文件仅用于安装、体验和正常使用软件。

## 下载与安装

前往本仓库右侧的 **Releases** 页面，下载最新版本：

```text
My_Capture9.3.exe
```

软件为单文件版本时，可以直接运行，无需安装 Python。

建议将程序放在固定目录，例如：

```text
C:\Program Files\My_Capture\
```

或：

```text
D:\Software\My_Capture\
```

不要长期放在下载目录中运行。后续移动 EXE 可能影响开机启动项、自定义图标路径或其他配置。

如果 Windows SmartScreen 显示警告，可在确认文件来自本仓库后选择：

```text
更多信息 → 仍要运行
```

## 主要功能

| 类别 | 功能 |
|---|---|
| 手动截图 | 单击候选区域截图，按住左键拖动可自由选择区域 |
| 窗口截图 | 默认优先识别整个窗口，并可切换到窗口内部区域 |
| 全屏截图 | 截取完整虚拟桌面，支持多显示器 |
| 内部区域识别 | 识别标题栏、工具栏、地址栏、目录树、侧边栏、内容区和状态栏 |
| 整窗优先 | `Space` 或 `W` 快速返回整个窗口，`I` 返回内部区域 |
| 候选切换 | 使用 `Tab`、`Shift+Tab` 或鼠标滚轮切换内外层候选 |
| 圆角处理 | A3-K2 纯二值圆弧逻辑，尽量保留 Windows 窗口真实透明圆角 |
| 屏幕实拍 | 保存屏幕上当前真实可见的像素 |
| 原窗口形状 | 在 Alpha 结果安全时保留窗口透明形状 |
| 下拉菜单截图 | 使用冻结画面保留下拉菜单，减少闪烁和菜单消失 |
| 光标保留 | 可在截图触发瞬间保留外部截图软件或系统光标 |
| 重截区域 | 按上一次区域快速再次截图 |
| 图库 | 在主窗口查看、选择、复制、删除和打开截图 |
| 图片信息栏 | 显示类型、文件大小、像素尺寸、截图时间及多选汇总 |
| 输出格式 | PNG、JPG、JPEG、BMP、WEBP、TIF、TIFF |
| 多语言 | English、简体中文、繁體中文、日本語 |
| 配色主题 | Explorer 浅色及多种深色、浅色主题 |
| 系统托盘 | 托盘截图、显示主界面、重截区域、打开目录、置顶和退出 |
| 开机启动 | 通过当前用户注册表启用，无需管理员权限 |
| 自定义图标 | 可更改主窗口、任务栏和托盘图标 |
| 调试支持 | 一键复制汇总调试信息，便于提交问题 |

## 默认快捷键

| 快捷键 | 功能 |
|---|---|
| `Ctrl + 1` | 手动截图 |
| `Alt + 3` | 活动窗口 / 窗口截图 |
| `Alt + 1` | 全屏截图 |
| `Delete` | 删除图库中选中的截图 |
| `Esc` | 退出截图选择器 |
| 鼠标右键 | 退出截图选择器 |

快捷键可在软件设置中修改或恢复默认值。

## 截图选择器操作

### 手动截图

- 单击高亮区域：截取当前候选。
- 按住左键拖动：截取自定义区域。
- `Tab` / `Shift+Tab`：切换候选。
- 鼠标滚轮：切换内层与外层候选。
- `Space` / `W`：切换到整个窗口。
- `I`：返回窗口内部区域。
- `Ctrl + 单击`：直接截取整个窗口。
- `Esc` / 鼠标右键：取消截图。

### 窗口截图

- 默认优先选中完整窗口。
- 使用 `Tab` 或滚轮切换窗口内部区域。
- 按 `Space` 或 `W` 随时返回整窗。
- 单击确认截图。

## 系统托盘

运行时会创建系统托盘图标。

托盘右键菜单包括：

- 显示主界面
- 手动截图
- 窗口截图
- 全屏截图
- 重截上一次区域
- 打开截图目录
- 复制汇总调试信息
- 总是在最前面
- 开机启动
- 退出 My_Capture

单击或双击托盘图标可显示或隐藏主窗口。

点击主窗口右上角关闭按钮时，软件默认最小化到托盘。需要完全退出时，请使用主界面“退出”或托盘菜单“退出 My_Capture”。

## 默认保存位置

默认截图目录：

```text
%USERPROFILE%\Pictures\My_Capture9.3
```

可以在软件中修改保存目录。

## 输出格式

支持保存为：

- PNG
- JPG / JPEG
- BMP
- WEBP
- TIF / TIFF

PNG 更适合需要透明圆角的窗口截图。JPG 不支持透明通道。

## 9.3 更新内容

- 新增开机启动选项，通过当前用户注册表启用，无需管理员权限。
- 运行时始终创建系统托盘图标。
- 新增完整的托盘右键菜单。
- 双击托盘图标可显示或隐藏主窗口。
- 点击关闭按钮默认最小化到托盘。
- 支持自定义主窗口、任务栏和托盘图标。
- 保留底部信息栏、整窗识别、内部区域识别、光标保留和 A3-K2 圆角逻辑。

## 近期版本重点

### 9.2

- 新增资源管理器风格的底部图片信息栏。
- 单选时显示类型、大小、尺寸和截图时间。
- 多选时显示数量、格式集合、总大小和时间范围。

### 9.1

- 手动截图和窗口截图均支持整窗与内部区域切换。
- 新增 `Space / W` 整窗、`I` 内部区域、`Ctrl + 单击` 整窗操作。
- 输出格式移动到工具栏算法列。
- 新增复制图片和重截区域。

### 9.0

- 新增窗口内部区域识别。
- 支持 Win32 子窗口识别和通用画面边界分割。
- 支持标题栏、工具栏、侧栏、内容区、状态栏等区域。

### 8.6–8.9

- 改进下拉菜单截图。
- 减少截图过渡闪烁。
- 修复本软件自截图和模态框卡死问题。
- 保留外部截图软件的光标状态。

### 8.0

- 使用 A3-K2 标准原位纯二值圆弧处理 Windows 圆角。

## 已知限制

- 软件主要针对 Windows 10 和 Windows 11。
- 部分 Electron、Qt 或自绘程序没有独立子窗口，内部区域识别需要依赖画面边界分析，结果可能因界面结构而不同。
- 受 DRM、硬件叠加层或受保护内容限制的窗口，可能无法被正常捕获。
- 不同 Windows 缩放比例、主题和软件自绘边框可能影响候选区域。
- JPG 格式不支持透明圆角。
- 多显示器使用不同 DPI 缩放时，建议先测试选框和最终截图是否完全一致。

## 问题反馈

请通过 GitHub **Issues** 提交问题，并尽量附上：

1. Windows 版本
2. 显示缩放比例
3. 软件版本
4. 截图模式
5. 操作步骤
6. 错误截图或录屏
7. 复制汇总调试信息得到的内容
8. 出问题的软件名称及版本

## 源代码与使用条件

本仓库仅用于发布 My_Capture 软件作品及更新。

- 源代码不公开。
- 未经作者明确许可，不得反编译、修改后重新发布、重新打包或冒用软件名称。
- 不得将本软件用于违法用途。
- 软件名称、Logo、界面设计和发布文件归作者所有。
- 个人用户可以下载并正常使用 Releases 中提供的软件版本。

---

# English

## About

**My_Capture 9.3** is a desktop screenshot tool for Windows 10 and Windows 11.

In addition to manual-region, window, and full-screen capture, it can detect internal window areas such as title bars, toolbars, address bars, sidebars, content panels, and status bars. It also includes rounded-corner processing, a screenshot gallery, an information bar, global hotkeys, multilingual UI, system tray integration, startup launch, and custom application icons.

This repository is used to:

- Publish finished application releases
- Provide release notes
- Display screenshots
- Distribute Windows executable files
- Collect bug reports and feature requests

The source code is **not publicly available**.

## Download and Installation

Open the repository's **Releases** page and download:

```text
My_Capture9.3.exe
```

The standalone executable can be launched directly without installing Python.

Place it in a fixed directory, for example:

```text
C:\Program Files\My_Capture\
```

or:

```text
D:\Software\My_Capture\
```

Avoid permanently running it from the Downloads folder because moving the executable later may affect startup registration, custom icon paths, or configuration.

## Features

| Category | Features |
|---|---|
| Manual capture | Click a detected region or drag to capture a custom rectangle |
| Window capture | Prioritizes the whole window and allows internal-region switching |
| Full-screen capture | Captures the full virtual desktop, including multi-monitor setups |
| Internal-region detection | Detects title bars, toolbars, address bars, trees, sidebars, content areas, and status bars |
| Whole-window shortcut | Use `Space` or `W` to return to the whole window; `I` returns to internal regions |
| Candidate switching | Use `Tab`, `Shift+Tab`, or the mouse wheel |
| Rounded corners | A3-K2 binary-arc processing for Windows rounded-window transparency |
| Screen pixels | Saves pixels currently visible on the screen |
| Original shape | Preserves transparent window shapes when the Alpha result is safe |
| Menu capture | Freezes the desktop to preserve open drop-down menus |
| Cursor preservation | Can preserve the cursor state at the capture trigger moment |
| Repeat region | Re-captures the previously selected rectangle |
| Gallery | View, select, copy, delete, and open captured images |
| Information bar | Shows type, size, dimensions, capture time, and multi-selection summaries |
| Output formats | PNG, JPG, JPEG, BMP, WEBP, TIF, TIFF |
| Languages | English, Simplified Chinese, Traditional Chinese, Japanese |
| Themes | Explorer Light and multiple dark/light color themes |
| System tray | Capture actions, main-window control, repeat region, folder access, always-on-top, and exit |
| Startup launch | Uses the current-user registry and does not require administrator rights |
| Custom icon | Changes the main-window, taskbar, and tray icon |
| Debug support | Copies a compact diagnostic bundle for issue reports |

## Default Hotkeys

| Shortcut | Action |
|---|---|
| `Ctrl + 1` | Manual capture |
| `Alt + 3` | Active-window / window capture |
| `Alt + 1` | Full-screen capture |
| `Delete` | Delete selected gallery items |
| `Esc` | Exit the capture selector |
| Right-click | Exit the capture selector |

Hotkeys can be changed or reset in Settings.

## Capture Selector Controls

### Manual Capture

- Click a highlighted region to capture it.
- Drag with the left mouse button to capture a custom rectangle.
- Use `Tab` / `Shift+Tab` to switch candidates.
- Use the mouse wheel to move between inner and outer candidates.
- Press `Space` / `W` to select the whole window.
- Press `I` to return to internal regions.
- Use `Ctrl + click` to capture the whole window directly.
- Press `Esc` or right-click to cancel.

### Window Capture

- The full window is selected first.
- Use `Tab` or the mouse wheel to switch to internal regions.
- Press `Space` or `W` to return to the whole window.
- Click to confirm.

## System Tray

The tray menu includes:

- Show main window
- Manual capture
- Window capture
- Full-screen capture
- Repeat last region
- Open screenshot folder
- Copy diagnostic summary
- Always on top
- Launch at startup
- Exit My_Capture

Clicking or double-clicking the tray icon shows or hides the main window.

Closing the main window normally minimizes the application to the tray. Use the main Exit command or **Exit My_Capture** from the tray to terminate it completely.

## Default Save Folder

```text
%USERPROFILE%\Pictures\My_Capture9.3
```

The folder can be changed in the application.

## Release Notes — 9.3

- Added launch-at-startup support without administrator privileges.
- Added a persistent system tray icon.
- Added a complete tray context menu.
- Added tray click/double-click main-window toggling.
- Closing the main window now minimizes it to the tray by default.
- Added custom main-window, taskbar, and tray icons.
- Preserved the information bar, whole-window detection, internal-region detection, cursor preservation, and A3-K2 rounded-corner logic.

## Known Limitations

- The application primarily targets Windows 10 and Windows 11.
- Electron, Qt, and custom-drawn applications may not expose native child windows, so internal-region detection may rely on visual boundary analysis.
- DRM-protected or hardware-overlay content may not be capturable.
- Different Windows DPI settings, themes, and custom borders may affect region detection.
- JPG does not support transparent corners.
- Mixed-DPI multi-monitor configurations should be tested for selector and output alignment.

## Bug Reports

Please use GitHub **Issues** and include:

1. Windows version
2. Display scaling percentage
3. Application version
4. Capture mode
5. Reproduction steps
6. Screenshot or screen recording
7. Copied diagnostic summary
8. Name and version of the affected application

## Source Code and Usage Terms

This repository is used only to publish My_Capture releases and updates.

- The source code is not published.
- Reverse engineering, modified redistribution, repackaging, or impersonation is not permitted without explicit authorization.
- The software must not be used for unlawful purposes.
- The application name, logo, interface design, and release files remain the property of the author.
- Individual users may download and use the versions provided through GitHub Releases.

---

# 日本語

## 作品概要

**My_Capture 9.3** は、Windows 10 / 11 向けのデスクトップスクリーンショットツールです。

手動範囲、ウィンドウ、全画面キャプチャに加え、タイトルバー、ツールバー、アドレスバー、サイドバー、内容領域、ステータスバーなど、ウィンドウ内部の領域を検出できます。角丸処理、キャプチャギャラリー、情報バー、グローバルショートカット、多言語 UI、システムトレイ、自動起動、カスタムアイコンにも対応しています。

このリポジトリは次の目的で使用します。

- 完成版ソフトウェアの公開
- リリースノートの提供
- スクリーンショットの掲載
- Windows EXE の配布
- 不具合報告と機能要望の受付

ソースコードは**公開していません**。

## ダウンロードとインストール

リポジトリの **Releases** ページから次のファイルをダウンロードしてください。

```text
My_Capture9.3.exe
```

単一 EXE 版は Python をインストールせずに実行できます。

固定フォルダーへの配置を推奨します。

```text
C:\Program Files\My_Capture\
```

または：

```text
D:\Software\My_Capture\
```

ダウンロードフォルダーから長期間実行すると、後で EXE を移動した際に自動起動、カスタムアイコン、設定パスへ影響する可能性があります。

## 主な機能

| カテゴリ | 機能 |
|---|---|
| 手動キャプチャ | 検出領域をクリック、またはドラッグして任意範囲を撮影 |
| ウィンドウキャプチャ | ウィンドウ全体を優先し、内部領域へ切り替え可能 |
| 全画面キャプチャ | マルチモニターを含む仮想デスクトップ全体を撮影 |
| 内部領域検出 | タイトルバー、ツールバー、アドレスバー、ツリー、サイドバー、内容領域、ステータスバー |
| ウィンドウ全体選択 | `Space` / `W` で全体、`I` で内部領域 |
| 候補切り替え | `Tab`、`Shift+Tab`、マウスホイール |
| 角丸処理 | Windows 角丸透明用の A3-K2 二値円弧処理 |
| 画面実写 | 画面上で現在見えているピクセルを保存 |
| 元ウィンドウ形状 | Alpha 結果が安全な場合に透明形状を保持 |
| メニュー撮影 | デスクトップを凍結し、開いたドロップダウンメニューを保持 |
| カーソル保持 | キャプチャ開始時点のカーソル状態を保持可能 |
| 前回範囲を再撮影 | 直前に選択した矩形を再キャプチャ |
| ギャラリー | 画像の表示、選択、コピー、削除、フォルダー表示 |
| 情報バー | 形式、サイズ、解像度、撮影時刻、複数選択の集計 |
| 出力形式 | PNG、JPG、JPEG、BMP、WEBP、TIF、TIFF |
| 多言語 | English、簡体字中国語、繁体字中国語、日本語 |
| テーマ | Explorer Light と複数のダーク / ライトテーマ |
| システムトレイ | 撮影、メイン画面、前回範囲、保存先、常に手前、終了 |
| 自動起動 | 現在のユーザーのレジストリを使用し、管理者権限は不要 |
| カスタムアイコン | メイン画面、タスクバー、トレイアイコンを変更 |
| デバッグ | 問題報告用の診断サマリーをコピー |

## 既定のショートカット

| ショートカット | 動作 |
|---|---|
| `Ctrl + 1` | 手動キャプチャ |
| `Alt + 3` | アクティブウィンドウ / ウィンドウキャプチャ |
| `Alt + 1` | 全画面キャプチャ |
| `Delete` | ギャラリーで選択した画像を削除 |
| `Esc` | キャプチャ選択画面を終了 |
| 右クリック | キャプチャ選択画面を終了 |

ショートカットは設定画面で変更または初期化できます。

## キャプチャ選択画面

### 手動キャプチャ

- 強調表示された領域をクリックして撮影します。
- 左ボタンでドラッグして任意範囲を撮影します。
- `Tab` / `Shift+Tab` で候補を切り替えます。
- マウスホイールで内側 / 外側の候補を切り替えます。
- `Space` / `W` でウィンドウ全体を選択します。
- `I` で内部領域へ戻ります。
- `Ctrl + クリック` でウィンドウ全体を直接撮影します。
- `Esc` または右クリックでキャンセルします。

### ウィンドウキャプチャ

- 最初にウィンドウ全体が選択されます。
- `Tab` またはホイールで内部領域へ切り替えます。
- `Space` または `W` で全体へ戻ります。
- クリックして確定します。

## システムトレイ

トレイメニュー：

- メイン画面を表示
- 手動キャプチャ
- ウィンドウキャプチャ
- 全画面キャプチャ
- 前回範囲を再撮影
- 保存先フォルダーを開く
- 診断サマリーをコピー
- 常に最前面
- Windows 起動時に実行
- My_Capture を終了

トレイアイコンのクリックまたはダブルクリックでメイン画面を表示 / 非表示にできます。

メイン画面の閉じるボタンを押すと、通常はトレイへ最小化されます。完全に終了するには、メイン画面の終了操作またはトレイの **My_Capture を終了** を使用してください。

## 既定の保存先

```text
%USERPROFILE%\Pictures\My_Capture9.3
```

保存先はアプリ内で変更できます。

## 9.3 リリースノート

- 管理者権限不要の自動起動を追加。
- 常駐システムトレイアイコンを追加。
- 完全なトレイ右クリックメニューを追加。
- トレイのクリック / ダブルクリックでメイン画面を切り替え。
- 閉じるボタンでトレイへ最小化。
- メイン画面、タスクバー、トレイのカスタムアイコンに対応。
- 情報バー、ウィンドウ全体検出、内部領域検出、カーソル保持、A3-K2 角丸処理を維持。

## 既知の制限

- 主に Windows 10 / 11 を対象としています。
- Electron、Qt、独自描画アプリではネイティブ子ウィンドウがない場合があり、画像境界解析を使用します。
- DRM 保護やハードウェアオーバーレイの内容は撮影できない場合があります。
- Windows の DPI、テーマ、独自枠線によって領域検出結果が変わる場合があります。
- JPG は透明な角丸を保持できません。
- 異なる DPI のマルチモニター環境では、選択枠と出力位置を事前に確認してください。

## 不具合報告

GitHub **Issues** に次の情報を添付してください。

1. Windows のバージョン
2. 表示スケール
3. アプリのバージョン
4. キャプチャモード
5. 再現手順
6. スクリーンショットまたは録画
7. コピーした診断サマリー
8. 問題が発生したソフト名とバージョン

## ソースコードと利用条件

このリポジトリは My_Capture の完成版と更新版を公開するためのものです。

- ソースコードは公開していません。
- 作者の明示的な許可なく、リバースエンジニアリング、改変版の再配布、再パッケージ化、名称の詐称を行わないでください。
- 違法な目的で使用しないでください。
- ソフトウェア名、ロゴ、UI デザイン、配布ファイルの権利は作者に帰属します。
- 個人ユーザーは GitHub Releases で提供されるバージョンをダウンロードして利用できます。

---

## Acknowledgements / 致谢 / 謝辞

- [PyQt5](https://www.riverbankcomputing.com/software/pyqt/)
- [Pillow](https://python-pillow.org/)
- Windows API / DWM / GDI

---

<p align="center">
  My_Capture 9.3<br>
  Windows Screenshot Tool / Windows 截图工具 / Windows スクリーンショットツール
</p>
