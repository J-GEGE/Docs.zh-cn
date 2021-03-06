---
title: 在 Visual Studio Code 中开始使用 ASP.NET Core Razor 页面
author: rick-anderson
description: 了解使用 Visual Studio Code 生成 ASP.NET Core Razor 页面 Web 应用的基础知识。
monikerRange: '>= aspnetcore-2.0'
ms.author: riande
ms.date: 08/27/2017
uid: tutorials/razor-pages-vsc/razor-pages-start
ms.openlocfilehash: b1f1dcc1401d707cff79f3269ab70b900e9fc21c
ms.sourcegitcommit: b8a2f14bf8dd346d7592977642b610bbcb0b0757
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/11/2018
ms.locfileid: "38123378"
---
# <a name="get-started-with-aspnet-core-razor-pages-in-visual-studio-code"></a>在 Visual Studio Code 中开始使用 ASP.NET Core Razor 页面

作者：[Rick Anderson](https://twitter.com/RickAndMSFT)

本教程介绍构建 ASP.NET Core Razor 页面 Web 应用的基础知识。 我们建议在学习本教程前先阅读 [Razor 页面介绍](xref:razor-pages/index)。 Razor 页面是在 ASP.NET Core 中为 Web 应用程序生成 UI 时建议使用的方法。

## <a name="prerequisites"></a>系统必备

[!INCLUDE [](~/includes/net-core-prereqs-vscode.md)]

## <a name="create-a-razor-web-app"></a>创建 Razor Web 应用

从终端运行以下命令：

::: moniker range=">= aspnetcore-2.1"

```console
dotnet new webapp -o RazorPagesMovie
cd RazorPagesMovie
dotnet run
```

[!INCLUDE[](~/includes/webapp-alias-notice.md)]

::: moniker-end

::: moniker range="= aspnetcore-2.0"

```console
dotnet new razor -o RazorPagesMovie
cd RazorPagesMovie
dotnet run
```

::: moniker-end

上述命令使用 [.NET Core CLI](https://docs.microsoft.com/dotnet/core/tools/dotnet) 创建并运行 Razor 页面项目。 打开浏览器，转到 http://localhost:5000 查看应用程序。

![主页或索引页](../razor-pages/razor-pages-start/_static/home.png)

[!INCLUDE [razor-pages-start](../../includes/RP/razor-pages-start.md)]

## <a name="open-the-project"></a>打开项目

按 Ctrl+C 关闭应用程序。

在 Visual Studio Code (VS Code) 中，选择“文件”>“打开文件夹”，然后选择“RazorPagesMovie”文件夹。

- 对警告消息“"RazorPagesMovie" 中缺少进行生成和调试所需的资产。是否添加它们?”选择“是” 。
- 对信息性消息“存在未解析的依赖项”选择“还原”。

### <a name="launch-the-app"></a>启动应用

按 Ctrl+F5 启动应用而不进行调试。 或者，从“调试”菜单中选择“开始执行(不调试)”。

在下一个教程中，我们将向项目添加模型。 

> [!div class="step-by-step"]
> [下一篇：添加模型](xref:tutorials/razor-pages-vsc/model)  
