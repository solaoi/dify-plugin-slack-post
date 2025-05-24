*他の言語で読む: [English](https://github.com/solaoi/dify-plugin-slack-post/blob/v0.0.1/README.md), [简体中文](https://github.com/solaoi/dify-plugin-slack-post/blob/v0.0.1/README.zh-Hans.md), [Português](https://github.com/solaoi/dify-plugin-slack-post/blob/v0.0.1/README.pt_BR.md).*

![license](https://img.shields.io/github/license/solaoi/dify-plugin-slack-post)

## Slack Post

<img width="120" alt="Image" src="_assets/icon.svg">

**Author:** solaoi
**Version:** 0.0.1
**Type:** 道具

### 解説

チャンネルやスレッドへのメッセージ投稿を行う、mrkdwn形式の表示に対応したSlackツールプラグイン。

<div align="left">
  <img src="_assets/how_to_use_0_ja.png" width="50%"/>
</div>

#### 機能

- スレッド内でのメッセージ投稿
- チャンネルへのメッセージ投稿
- Slack 上での `mrkdwn` フォーマットに対応

#### 1. インストール方法

「プラグインをインストールする」画面で、以下のGitHubリポジトリを指定してインストールしてください。

https://github.com/solaoi/dify-plugin-slack-post

#### 2. 設定手順

##### 2-1. 公式のSlackBotプラグインと同様の手順でBot Tokenを作成します。

##### 2-2. 本プラグインの利用には、以下のスコープが必要です。

```text
chat:write
```

##### 2-3. 公式のSlackBotプラグインのセットアップ手順については以下をご参照ください。

https://github.com/langgenius/dify-official-plugins/blob/main/extensions/slack_bot/README.md

#### 3. 使い方

##### 3.1. Slackチャンネルへの投稿

<div align="left">
  <img src="_assets/how_to_use_1_ja.png" width="50%"/>
</div>

| 入力変数 | 説明 |
| ---- | ---- |
| channel_id | Slack チャンネルID |
| content | チャンネルに投稿するメッセージ内容 |

##### 3.2. Slackスレッドへの投稿

<div align="left">
  <img src="_assets/how_to_use_2_ja.png" width="50%"/>
</div>

| 入力変数 | 説明 |
| ---- | ---- |
| thread_ts | Slack スレッドTS |
| channel_id | Slack チャンネルID |
| content | スレッドに投稿するメッセージ内容 |

#### 4. オプション

以下の拡張機能プラグインを併用すると、投稿先のパラメータ（チャンネルID及びスレッドTS）を簡単に取得できます。

- Slack Thread Bot  
https://marketplace.dify.ai/plugins/solaoi/slack-thread-bot
