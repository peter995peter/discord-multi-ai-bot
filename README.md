# discord-multi-ai-bot
使用OpenAI API格式製作的多模型Discord聊天機器人

## 安裝教學
1. 設定 `config/config.json`
2. 設定 `config/model.json`
3. 安裝必要套件:
```
pip install -r requirements.txt
```
4. 啟動機器人
```
python3 bot.py
```

## 檔案設定
> config/config.json
* `token`: 你的機器人token，可以前往[Discord Developer Portal](https://discord.com/developers/applications)創建
* `owner_name`: 有人問開發者是誰的時候會回覆的名稱
* `prefix`: 指令的前綴，如果設定成`m@`設定頻道指令就是`m@set`
* `default_model`: 第一次和機器人對話時要用什麼模型回答，必須在`config/model.json`的`models`裡面

> config/model.json
* `api`:
  * `url`: 生成回覆的api(必須使用OpenAI API格式）
  * `key`: api key，獲取教學請看[取得API Key](#取得api-key)，若無可以不修改
* `models`: "模型名稱": "api 提供者"(如果你沒有要新增模型基本上不用動）

## 取得API Key
* [Gemini](https://aistudio.google.com/apikey)
* [Grok](https://console.x.ai)
* [OpenAI](https://platform.openai.com/settings/organization/api-keys)
