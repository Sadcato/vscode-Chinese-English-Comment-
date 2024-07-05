# 中英文注释翻译器

![here.png](images/here.png)

## 概述

“中英文注释翻译器”是一个 Visual Studio Code 扩展，它提供实时的中英双向注释翻译功能，帮助开发者在多语言环境下提高代码的可读性和理解性。  
该扩展支持使用 `Ctrl+Y` 将中文注释翻译为英文，并支持使用 `Alt+Y` 将英文注释通过悬浮提示翻译为中文。使用本插件前，您需要配置有道智能云的 API ID 和密钥。

## 配置

在使用本插件之前，您需要在有道智能云注册账户并创建应用以获取 API ID 和密钥。将这些信息填入 `extension.ts` 文件的指定位置以启用翻译功能。

### 获取 API 密钥

1. 访问 [有道智能云](https://ai.youdao.com/) 并登录或注册新账户。
2. 创建一个新应用并获取您的 API ID 和 API 密钥。
3. 将获取的 API ID 和密钥填入以下位置：

```typescript
const appKey = "YOUR_APP_ID"; // 替换 YOUR_APP_ID 为您的应用 ID
const appSecret = "YOUR_APP_SECRET"; // 替换 YOUR_APP_SECRET 为您的应用密钥
```

## 功能特点

中文翻译至英文：选中中文注释后，按 Ctrl+Y 即可自动翻译为英文，并在下一行显示。  
悬浮翻译英文至中文：选中英文文本后，按 Alt+Y 即可在悬浮窗口中显示中文翻译，这种方式既便捷又不干扰代码阅读。

## 安装方法

此扩展可以直接从 Visual Studio Code Marketplace 安装：
打开 Visual Studio Code。  
通过点击侧边栏上的方块图标或按 Ctrl+Shift+X 打开扩展视图。  
搜索 “中英文注释翻译器”。
点击安装按钮。

## 使用说明

对于中文至英文的翻译：  
选中代码中的中文注释。  
按 Ctrl+Y。  
翻译后的英文注释将出现在下一行。  
![cn2en.png](images/cn2en.png)

对于英文至中文的翻译：  
选中需要翻译的英文文本。  
按 Alt+Y。  
一个包含中文翻译的悬浮提示将显示在所选文本上。  
![en2cn.png](images/en2cn.png)

## 已知问题

目前，如果网络存在问题，翻译可能会出现延迟或错误，因为它依赖于外部 API。

## 贡献

欢迎为 “中英文注释翻译器” 做出贡献！如果您有改进的建议或发现了错误，请在我们的 [GitHub](https://github.com/Sadcato/vscode-Chinese-English-Comment-translator) 仓库中开启一个问题或提交一个合并请求。

欢迎给我们的项目点点 Star ✨

## 许可证

该扩展在 MIT 许可证下发布。扩展随附的 LICENSE 文件中提供了完整的许可证文本。

## 支持

如需支持、功能请求或更多信息，请访问 我们的 [GitHub](https://github.com/Sadcato/vscode-Chinese-English-Comment-translator) 仓库 或在那里开启一个问题。
