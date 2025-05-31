# Sample 项目 - Nez 引擎示例

本 README 文档旨在帮助您理解和运行此 Nez 引擎示例项目。

## Sample 项目用途

本项目展示了如何在 Nez 引擎中创建一个基本的窗口、加载资源以及实现一个简单的场景。它为您提供了一个起点，您可以在此基础上构建自己的游戏或应用程序。


## 先决条件

- [.NET 9 SDK](https://dotnet.microsoft.com/download/dotnet/9.0) 或更高版本
- 兼容的集成开发环境 (IDE)，例如：
    - Visual Studio 2022
    - JetBrains Rider
    - Visual Studio Code (带有 C# 扩展)

<!-- 如果有其他特定依赖，请在此处列出 -->

## 如何运行

1.  **克隆或下载仓库**:
```bash
    # 以模板库的形式克隆或下载
    git clone https://github.com/ProjektMing/Nez-Template.git
    cd Nez-Template
    # 更新上游 FNA 和 Nez 子模块
    git submodule update --init --recursive
```
2.  **确认依赖**:
      参考 [本文](./fnalibs/README.md) 内容，确保 `fnalibs` 文件夹中包含了 FNA 引擎所需的库文件。
      
      可选：要求安装 Vulkan SDK，但若只看效果，FNA 也可以在没有 Vulkan 的情况下运行。

3.  **恢复 .NET 依赖**:
    打开终端或命令提示符，导航到 `Sample` 项目目录 (包含 `Sample.csproj` 文件的目录)，然后运行：
```bash
    dotnet restore
```

4.  **构建项目**:
```bash
    dotnet build
```

5.  **运行项目**:
```bash
    dotnet run
```

或者，您可以直接在您的 IDE 中打开并运行 `Sample.csproj` 项目。

## 项目结构说明

本 Sample 项目的结构部分参考了 [FNA-VSCode-Template](https://github.com/prime31/FNA-VSCode-Template/tree/master) 项目。

## 代码概览

以下是 `Sample` 项目中的一些关键文件和目录：

-   `Program.cs`: 应用程序的入口点，负责初始化并运行游戏。
-   `Game.cs`: 继承自 `Nez.Core`，是游戏的主要类，用于设置全局游戏属性和初始场景。
-   `Scenes/`: 此目录通常包含游戏的不同场景。
    -   `SplashScene.cs`: (如果存在) 一个示例场景，通常用于显示启动画面或主菜单。

<!-- 根据实际项目结构和内容，调整或添加更多关于代码组织和关键组件的说明 -->

## 自定义与后续步骤

您可以基于此示例项目进行以下操作：

-   **探索 Nez 功能**: 查阅 [Nez 引擎官方文档](https://github.com/prime31/Nez) (请注意，Nez 的文档可能主要在 GitHub 上) 来了解更多关于场景管理、实体、组件、图形渲染、输入处理等功能。
-   **创建新场景**: 在 `Scenes/` 目录下添加您自己的场景。
-   **添加游戏逻辑**: 修改现有的实体和组件，或者创建新的实体和组件来实现您的游戏玩法。
-   **集成其他 Nez 扩展**: Nez 社区可能提供了一些有用的扩展或工具，您可以考虑将它们集成到您的项目中。

祝您开发愉快！
