## [English User Manual](README.en-US.md)

# [公益]AIChatPlugin - Terraria 插件

## 概述

AIChatPlugin 是一个为 Terraria 游戏服务器设计的插件，它允许玩家通过聊天与一个 AI 对话系统进行互动。该插件提供了一个简单的接口，使得玩家可以通过特定的命令或聊天触发词来向 AI 提出问题，并接收回答。

## 功能特点

- **命令触发**：玩家可以通过命令或聊天触发词来激活 AI 对话。
- **上下文管理**：插件会记录玩家的对话上下文，以便提供更连贯的回答。
- **配置灵活**：通过配置文件，管理员可以自定义 AI 的行为，包括触发词、回答字数限制等。
- **帮助命令**：内置的帮助命令可以帮助玩家了解如何使用插件。
- **重置功能**：玩家可以通过命令重置自己的对话上下文。
- **联网搜索**：根据配置，AI 可以启用联网搜索功能来增强回答。
- **消息转发**：支持将消息转发到指定的 QQ 群聊。

## 安装步骤

1. 将 AIChatPlugin 插件文件放置在 ServerPlugins 插件目录下。
2. 确保你的 Terraria 服务器已经安装并运行 TShock。
3. 重启 TShock 以加载插件。

## 使用方法

- **激活 AI 对话**：在聊天栏输入 `AI` 或其他自定义的触发词，然后输入你的问题。
- **发送命令**：
  - `/ab`：向 AI 提问。
  - `/bcz`：清除你的上下文记录。
  - `/bbz`：显示帮助信息。
  - `/aiclearall`：管理员命令，清除所有玩家的上下文记录。

## 配置文件

AIChatPlugin 使用一个 JSON 格式的配置文件，位于 `tshock` 目录下，名为 `AI聊天配置.json`。你可以编辑此文件来自定义插件的行为：

- **模型**：选择 AI 模型，1 为通用，2 为速度。
- **触发提示词**：定义触发 AI 对话的关键词。
- **回答字限制**：设置 AI 回答的最大字数。
- **回答换行字**：设置 AI 回答自动换行的字数。
- **上下文限制**：设置每个玩家上下文记录的最大数量。
- **联网搜索**：是否允许 AI 进行联网搜索。
- **转发QQ群总开关**：是否启用消息转发到 QQ 群聊的功能。
- **转发QQ群**：指定要转发消息的 QQ 群号。
- **设定**：自定义 AI 的行为设定。
- **temperature温度**：设置 AI 回答的温度参数。
- **top_p核采样**：设置 AI 回答的 top_p 参数。

## 注意事项

- 确保你的服务器网络连接正常，以便 AI 能够访问必要的 API。
- 如果你不希望使用消息转发功能，请确保相关配置项为关闭状态。

## 贡献与支持

如果你有任何问题或建议，欢迎通过 GitHub 提交 issue 或 pull request。同时，你也可以联系插件作者：镜奇路蓝。
