---
title: "📝 note"
date: 2023-08-04
description: "メモです"
summary: "メモです"
---

特設サイト作成時のメモです．

## 導線について
当初，profileModeのボタンからREADMEページに誘導していたが，テストユーザーからのフィードバックで
- ボタンだと分かりにくい
- 他にも多くのボタンがあり，READMEへの誘導ボタンを押そうと思わない
- READMEページに到達することなくページを閉じてしまう

といった指摘を頂いた．

そこで，profileの下部（読み込んだ後，スクロールしなくても見える範囲）に記事一覧を表示させることで，ホーム画面以外にもコンテンツがあることを示し，この問題を解決しようと試みた．

しかし，デフォルトではprofileModeだと記事一覧は表示されない．以下の変更を行うことで，無理やりprofileModeにも記事一覧を表示させることに成功した．
- `layouts/_default/list.html`のif-statementを変更
- READMEページを`content/posts/`に配置

また，追加でトップ画面読み込み時にスクロールダウンさせるJavaScriptを挿入した．
これにより，READMEページにたどり着くユーザーの増加が期待できる．

## emoji
> <https://www.webfx.com/tools/emoji-cheat-sheet/>
