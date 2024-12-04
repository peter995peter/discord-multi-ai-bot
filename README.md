# discord-multi-ai-bot
使用OpenAI API格式製作的多模型Discord聊天機器人

## 安裝教學
1. 設定`config/config.json`

## 檔案設定
> config/config.json

* `token`: 你的機器人token，可以前往[Discord Developer Portal](https://discord.com/developers/applications)創建
* `owner_name`: 有人問開發者是誰的時候會回覆的名稱
* `prefix`: 指令的前綴，如果設定成`m@`設定頻道指令就是`m@set`
* `default_model`: 第一次和機器人對話時要用什麼模型回答，必須在`config/model.json`裡面
