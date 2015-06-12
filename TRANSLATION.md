Translation Note
================

_Note: This docs is written in Japanese_

## 翻訳について

[atom/electron](https://github.com/atom/electron)の[Docs/](https://github.com/atom/electron/tree/master/docs)以下を翻訳します。

翻訳をするものについては、できるだけ内容の更新頻度が低い _Guides_ や _Tutorials_ を優先する。もちろんすべての翻訳ができることが理想ではあるが、翻訳が追いつかず元のドキュメントと比べて古いものが残りユーザーを混乱させてしまうことは避けたい。ある程度 _API_ の更新頻度が落ち着いてきたら再度この問題について考える予定です。

## 翻訳フロー

`atom/electron.atom.io`で`atom/electron/docs`内の日本語翻訳については「[Translation in Japanese #20](https://github.com/atom/electron.atom.io/issues/20)」でその方法について話し合われ翻訳は以下のようにします。

1\. atom/electronをクローン：

```bash
$ git clone git@github.com:atom/electron.git
```

2\. 翻訳するドキュメントごとにブランチを作成：

```bash
$ git checkout -b translate/<document>-jp
```

3\. 翻訳するドキュメントごとに新しいファイルを作成：

```bash
$ cp /path/to/<document>.md /path/to/<document>-jp.md
```

また、今後誰もが簡単に翻訳ができるようにガイドラインの作成についても「[Create a guide for translation #28](https://github.com/atom/electron.atom.io/issues/28)」で話し合っています。

## 翻訳ルール

翻訳については、Oracle の斎藤玲子さんによる[日本語スタイルガイドクイックリファレンス](https://blogs.oracle.com/reiko/resource/ja-style-quick.pdf)を参考にしています。

## 翻訳一覧

### ガイド

ドキュメント                        | ステータス        | 担当
--------------------------------- | --------------- | -------------  
[Application distribution][1]     |                 |  (not assigned)
[Application packaging][2]        |                 | (not assigned)
[Using native node modules][3]    |                 | (not assigned)
[Debugging main process][4]       |                 | (not assigned)
[Using Selenium and WebDriver][5] |                 | (not assigned)
[DevTools extension][6]           |                 | (not assigned)
[Using pepper flash plugin][7]    |                 | (not assigned)

[1]: https://github.com/atom/electron/blob/master/docs/tutorial/application-distribution.md
[2]: https://github.com/atom/electron/blob/master/docs/tutorial/application-packaging.md
[3]: https://github.com/atom/electron/blob/master/docs/tutorial/using-native-node-modules.md
[4]: https://github.com/atom/electron/blob/master/docs/tutorial/debugging-main-process.md
[5]: https://github.com/atom/electron/blob/master/docs/tutorial/using-selenium-and-webdriver.md
[6]: https://github.com/atom/electron/blob/master/docs/tutorial/devtools-extension.md
[7]: https://github.com/atom/electron/blob/master/docs/tutorial/using-pepper-flash-plugin.md


### チュートリアル

ドキュメント                           | ステータス        | 担当
------------------------------------ | --------------- | -------------  
[Quick start][1]                     |  PR             | Sota Yamashita
[Desktop environment integration][2] |  翻訳中          | Sota Yamashita
[Online/offline event detection][3]  |                 | (not assigned)


[1]: https://github.com/atom/electron/blob/master/docs/tutorial/quick-start.md
[2]: https://github.com/atom/electron/blob/master/docs/tutorial/desktop-environment-integration.md
[3]: https://github.com/atom/electron/blob/master/docs/tutorial/online-offline-events.md

## 翻訳ヒント

* Quick start ↔ クイックスタート
* Introduction ↔ 導入
* Main Process ↔ メインプロセス
* Renderer process ↔ リレンダラープロセス
