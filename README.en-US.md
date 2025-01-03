## AIChatPlugin - Terraria Plugin

## Overview

AIChatPlugin is a plugin for the Terraria game server that allows players to interact with an AI dialog system via chat. The plugin provides a simple interface that allows players to ask the AI questions and receive answers via specific commands or chat trigger words.

## Features

- **Command Trigger**: Players can activate AI conversations via commands or chat trigger words.
- **Context Management**: The plugin records the context of the player's conversations in order to provide more coherent answers.
- **Configuration Flexibility**: Through the configuration file, administrators can customize the behavior of the AI, including trigger words, answer word limits, etc.
- **Help Commands**: Built-in help commands help players understand how to use the plugin.
- **Reset Function**: Players can reset their dialog context through commands.
- **Networked Search**: Depending on the configuration, the AI can enable the networked search feature to enhance answers.
- **Message Forwarding**: Supports forwarding messages to specified QQ group chats.

## Installation Steps

1. Place the AIChatPlugin plugin file in the ServerPlugins plugin directory.
2. Ensure that your Terraria server has TShock installed and running. 3.
3. Restart TShock to load the plugin.

## Usage

- **Activate AI Conversation**: Type `AI` or another customized trigger word in the chat field and type your question.
- **Send command**:
  - `/aibot` or `/ab`: Ask the AI a question.
  - `/botreset`: clear your context record.
  - `/bothelp`: show help messages.
  - `/clearAllcontext`: administrator command that clears all players' context records.

## Configuration files

The AIChatPlugin uses a JSON-formatted configuration file, located in the `tshock` directory, called `AIChatConfig.json`. You can edit this file to customize the behavior of the plugin:

- **模型选择**: selects the AI model, 1 for generic, 2 for speed.
- **聊天触发AI提示词**: define the keyword to trigger AI dialog.
- **AI回答字数限制**: set the maximum number of words for AI answer.
- **AI回答换行字数**: Set the number of characters for AI answer to automatically break lines.
- **上下文限制**: Set the maximum number of context records per player.
- **启用联网搜索**: Whether to allow AI to perform network search.
- **AI设定**: customize the behavior of AI.
- **temperature温度**: set the temperature parameter for AI to answer.
- **top_p核采样**: set the top_p parameter of AI response.

## Notes

- Make sure your server network connection is working so that the AI can access the necessary APIs.
- If you encounter problems, check that the configuration file is properly configured and that the API key is valid.
- If you do not wish to use the message forwarding feature, make sure the relevant configuration item is turned off.

## Contribute and support

If you have any questions or suggestions, please feel free to submit an issue or pull request via GitHub, and you can also contact the plugin's author, Mirrorchild Blue.