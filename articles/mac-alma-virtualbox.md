---
title: "Apple Silicon & VirtualBox 7でAlmaLinuxをインストール時の注意点"
emoji: "⛳"
type: "tech" # tech: 技術記事 / idea: アイデア
topics: ["Mac", "VirtualBox", "AlmaLinux", "ARM64"]
published: true
---
# はじめに

Apple Silicon搭載のMacでVirtualBox 7を使用して、AlmaLinux (ARM64版) をインストールするときの注意点。

# 必要な環境

- Apple Silicon搭載のMac
- VirtualBox 7
- AlmaLinuxのARM64版ISO  

https://almalinux.org/ja/get-almalinux/

# インストールの注意点

1. ISOとしてダウンロードしたARM64版のAlmaLinuxを指定します。
2. OSの選択時に **Fedora** を選びます。（RedHat系オプションがないため）
3. 仮想マシンを起動します。

# その他

- 画面サイズが小さい場合、適宜ディスプレイ設定の倍率をあげる。（200%程度）