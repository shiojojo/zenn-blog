---
title: "macOSにおけるVSCodeでのcmd＋番号によるタブ切替"
emoji: "🐕"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["VSCode", "macOS", "ショートカット"]
published: true
---
# 概要
- 本記事は、macOS上でVSCodeのタブ切替をカスタマイズする方法を解説します。
- デフォルトでは、control+番号がエディタ切り替え、cmd+番号がグループ切り替えです。
- この記事では、cmd+番号でエディタタブを切り替える設定を紹介します。

## ショートカット設定

以下のコードを `keybindings.json` に追加してください。

```json
[
    {
        "key": "cmd+1",
        "command": "workbench.action.openEditorAtIndex1"
    },
    {
        "key": "cmd+2",
        "command": "workbench.action.openEditorAtIndex2"
    },
    {
        "key": "cmd+3",
        "command": "workbench.action.openEditorAtIndex3"
    },
    {
        "key": "cmd+4",
        "command": "workbench.action.openEditorAtIndex4"
    },
    {
        "key": "cmd+5",
        "command": "workbench.action.openEditorAtIndex5"
    },
    {
        "key": "cmd+6",
        "command": "workbench.action.openEditorAtIndex6"
    },
    {
        "key": "cmd+7",
        "command": "workbench.action.openEditorAtIndex7"
    },
    {
        "key": "cmd+8",
        "command": "workbench.action.openEditorAtIndex8"
    },
    {
        "key": "cmd+9",
        "command": "workbench.action.openEditorAtIndex9"
    }
]
```

### 手順
1. VSCodeで **Cmd + Shift + P** を押してコマンドパレットを開く  
2. コマンドパレットに「Open Keyboard Shortcuts (JSON)」と入力し、Enter キーを押して `keybindings.json` を開く  
3. 上記の設定を追加し、保存  
4. VSCodeを再起動

# まとめ
これで、VSCodeのタブ切替用ショートカットが設定されます。
