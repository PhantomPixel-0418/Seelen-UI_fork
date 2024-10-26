<h1 align="center">
  <img src="documentation/images/logo.svg" width="44" align="top" alt="Seelen UI Logo" />
  Seelen UI
</h1>

- [English](/README.md)
- [中文](/docs/README.zh.md)
- [Français](/docs/README.fr.md)
- [Español](/docs/README.es.md)
- [Deutsch](/docs/README.de.md)

<h2 align="center">
  完全可定制的 Windows 桌面环境
  <br/>
  支持 70 多种语言
</h2>

<div align="center"> 

[![Contributors](https://img.shields.io/github/contributors/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/graphs/contributors)
[![Last Commit](https://img.shields.io/github/last-commit/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/commits/main)
[![Version](https://img.shields.io/github/v/release/eythaann/seelen-ui.svg)](https://github.com/eythaann/seelen-ui/releases)
[![Downloads](https://img.shields.io/github/downloads/eythaann/seelen-ui/total.svg)](https://github.com/eythaann/seelen-ui/releases)

</div>

<img src="./documentation/images/preview.png" width="100%" alt="Seelen UI 桌面截图，展示了自定义的桌面环境">

## 目录
- [概述](#overview)
- [安装](#installation)
  - [Microsoft Store（推荐）](#microsoft-store-emrecommendedem)
  - [Winget](#winget)
  - [.msix 安装包](#msix-installer)
  - [.exe 安装程序](#exe-installer)
- [使用方法](#usage)
- [即将推出的功能](#upcoming-features)
- [文档](#documentation)
  - [语言](./documentation/languages.md)
  - [工具栏](./documentation/toolbar.md)
  - [主题](./documentation/themes.md)
  - [窗口管理器](./documentation/window_manager.md)
  - [项目](./documentation/project.md)
- [贡献](#contributing)
- [许可](#license)
- [联系方式](#contact)

## 概述
Seelen UI 是一个设计用于提升 Windows 桌面体验的工具，专注于自定义和生产力。它能够平滑地集成到系统中，提供一系列功能，让您可以个性化桌面并优化工作流程。

* **定制您的桌面**：Seelen UI 允许您根据自己的风格和需求调整桌面。您可以调整菜单、窗口小部件和其他元素，创建适合您的工作空间。

  ![Seelen UI 简约桌面](./documentation/images/preview2.png)

<br/>

* **提升您的生产力**：Seelen UI 帮助您高效组织桌面。通过平铺窗口管理器，窗口将自动排列，支持多任务处理，使工作更加流畅。

  ![Seelen UI 平铺窗口管理器](./documentation/images/twm_preview.png)

<br/>

* **享受您的音乐**：Seelen UI 集成了兼容大多数音乐播放器的媒体模块，您可以随时播放、暂停和跳过曲目，无需打开额外窗口。

  ![Seelen UI 媒体模块](./documentation/images/media_module_preview.png)

<br/>

* **加速工作**：通过 Rofi 启发的应用启动器，Seelen UI 提供了一种快速访问应用程序和执行命令的简单直观方式。

  ![Seelen UI 应用启动器](./documentation/images/app_launcher_preview.png)

<br/>

* **用户友好的配置**：Seelen UI 提供了直观的界面，方便定制设置，如主题、任务栏布局、图标等，只需轻松点击几下。

  ![Seelen UI 设置](./documentation/images/settings_preview.png)

<br/>

## 安装
> **⚠️ 注意**：Seelen UI 需要安装 WebView 运行时。Windows 11 自带此功能，但在 Windows 10 上需要单独安装。安装程序还需要 Microsoft Edge 正常运行。如果您的系统中移除了 Edge，请确保 Edge 和 WebView 运行时已安装。

> **🗒️ 提示**：在全新安装的 Windows 系统中，应用可能显示黑屏或白屏。您只需通过 Windows Update 更新系统并重新启动即可。

您可以选择以下不同的安装选项：

### Microsoft Store <em>(推荐)</em>
从 [商店](https://www.microsoft.com/store/productId/9P67C2D4T9FB?ocid=pdpshare) 页面下载最新版本。这是推荐的选项，因为您将收到更新，并且程序版本安全。

***注***：由于商店中更新需要人工审核，通常花费 1 至 3 个工作日生效。

### Winget
使用以下命令安装最新版本：

``` pwsh
winget install --id Seelen.SeelenUI
``` 

此选项还使用签名的 `.msix` 软件包，确保您拥有最新的安全版本。与微软商店类似，Winget 中可能需要 1 到 3 个工作日才能反映出更改，因为更新是由 `winget-pkg` 项目中的人工批准的。

### .msix 安装包
从 [发布页面](https://github.com/eythaann/seelen-ui/releases) 下载 `.msix` 安装包。此包已签名，确保安装过程的安全性。

### .exe 安装程序
从 [发布页面](https://github.com/eythaann/seelen-ui/releases) 下载最新版本并运行 `setup.exe` 安装程序。此选项不推荐，因为安装程序未签名，可能被部分杀毒软件标记为潜在威胁。

## 使用方法

安装或解压后，打开程序。简单直观的图形界面将引导您配置设置，轻松个性化桌面环境。

## 文档

有关 Seelen UI 各方面的详细信息，请查阅以下文档：
- [语言](./documentation/languages.md) - 了解翻译相关信息。
- [工具栏](./documentation/toolbar.md) - 自定义和使用工具栏指南。
- [主题](./documentation/themes.md) - 指南如何创建和应用主题。
- [窗口管理器](./documentation/windows_manager.md) - 配置窗口管理器说明。
- [项目](./documentation/project.md) - 项目信息概览。

## 即将推出的功能

我很高兴与大家分享 Seelen UI 的一些即将推出的功能！以下是未来功能的预览：

### ~~应用启动器~~ ✅
我计划开发一个应用启动器，灵感来自于 [Rofi](https://github.com/davatorium/rofi)（Linux 平台）。该功能将提供一种快速访问应用程序的简洁方式。

![App Launcher Preview](https://raw.githubusercontent.com/adi1090x/files/master/rofi/previews/colorful/main.gif)
*图片由 [rofi-themes](https://github.com/dctxmei/rofi-themes) 提供*


### 自定义弹出小部件
我计划推出一组完全可自定义的弹出小部件，类似于 [EWW](https://github.com/elkowar/eww) 提供的功能。小部件将高度可配置，适应您的需求，提供更佳的交互体验。

![Customizable Widgets Preview](https://raw.githubusercontent.com/adi1090x/widgets/main/previews/dashboard.png)
*图片由 [adi1090x](https://github.com/adi1090x/widgets) 提供*

### 自定义 Alt + Tab（任务切换）
即将推出的升级版 Alt + Tab 系统将提供更直观的任务切换体验。

### 自定义虚拟桌面查看器和动画
我们正在开发自定义虚拟桌面查看器和动态动画，以改善不同工作区之间的导航体验。

敬请关注更新！感谢您的支持与热情！

Seelen UI 团队

## 贡献

欢迎大家贡献！
* 阅读 [贡献指南](CONTRIBUTING) 以了解开始的条款。
* 查看 [项目文档](documentation/project.md) 以了解项目结构。

## 许可证

请查看 [LICENSE](LICENSE) 文件了解详细信息。

## 联系方式

如有帮助或有疑问，请通过 [Discord](https://discord.gg/ABfASx5ZAJ) 联系我们。

## 再见
```
                   .      .&     _,x&"``
                    & .   &'  ;.&&'
              &.  . &.&     .0&&&;&""`
         .    '&  &.&&&  .&&&&&'
       .&         ;&&& &&&&&'
      &&          &&&&&&&&     &&&
     0&    .     &&&&&&&&""
    &&   .0     &&&&&&&
   0&& .&'     &&&&&&
  :&&&&&    . &&&&& 
  0&&&&    & &&&&&
  &&&&'   &&&&&&&               .&&&x&
  &&&&   :&&&&&0.&'        , .&&&&&&&&&&;.
  &&&&.  &&&&&&&&        .&&&&&&&&&&'               .
  0&&&&  &&&&&&&       ,&&&&&&&&&&&&                &
  :&&&&; &&&&&0       ,;&&&&&&&&&&&             ;  .0
   0&&&&&&&&&&0     ,;&&&&&&&&&&&&&             &  &;
    0&&&&&&&&&&0   :',;".&&&&&&".&             && &0
     0&&&&&&&&&0  ',;',&&&&&" ,&'             &&&&0
      0&&&&&&&&&0 ,x&&&&" .&&&              &&&&0
        0&&&&&& .&&&&"'''"&&"&&            &&&&&0
         0&& .&&;``       `&: :&         &&&&&&0
            &"' &&&&&&&&   &"& &"&   &&&&&&&&0
              0&&&&&&&&&&&&&&&&&&&&&&&&&0
                 0&&&&&&&&&&&&&&&&&&&0         Seelen
                      0&&&&&&&&&0
```
