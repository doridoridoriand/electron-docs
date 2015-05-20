Documentation for Electron
==========================

TL;DR

>Electron is the cross-platform application shell we originally built for the Atom editor to handle the Chromium/Node.js event loop integration and native APIs.

Electronはクロスプラットフォームアプリケーションシェル。もともとはChromium/Node.jsのevent loop integrationやネイティブAPIをAtomエディタで使うために作られました。

* Documentation for Electron
 * Electronとは
 * Electronの構成
 * アプリケーションの設計
 * 実行プロセス
 * Main Process と Renderer Processのブリッジ
 * モジュール
 * 新しいDOM要素作成
 * 内部構成
    * Main Process と Renderer Process
    * Sandboxing化されない
    * ChromiumとNode.js
    * Main Process と Renderer Processのブリッジ
* リソース
 * 情報を得る方法
 * 類似ツール
 * 参考サイト
* その他
 * ドキュメントの翻訳方法
* タスク
* コントリビュート
* ライセンス

## Electronの構造

## リソース

Electronについて調べる際は以下のサイトがとても参考になります:

* [Electron公式ページ](http://electron.atom.io/) - Electronの公式ページ。ここではチュートリアルやドキュメントを見ることができます。
* [@electronjs](https://twitter.com/electronjs) - ElectronのTwitterアカウント
* [Discuss about Electron](https://discuss.atom.io/c/electron) - AtomのDiscussページなります。Electronについて話合われています。
* [Awesome Electron](https://github.com/sindresorhus/awesome-electron) - [Sindre Sorhus](https://github.com/sindresorhus/)によって作成されたElectron関連のまとめす。
* [atom-slack](http://atom-slack.herokuapp.com/) - Atom全般のことについて話合われています。`#electron`ルームもあります。

Electronの前の名前はAtom-shellです。名前を変えただけなので、Electronについて検索する際は`Atom-shell`で検索したほうがQiitaなどでも多くの記事を見つけることができます。以下はQiita上のタグ一覧です。

* [#atom-shell](http://qiita.com/tags/atom-shell)
* [#electron](http://qiita.com/tags/electron)

### 参考サイト

* [Atom Shell is now Electron](http://blog.atom.io/2015/04/23/electron.html) - Atom-shellからElectronに名前を変更したことのリリースです。
* [GitHub、JavaScriptでデスクトップアプリが作れるライブラリAtom Shellを、Electronに改称](http://codezine.jp/article/detail/8678) - 公式リリースの簡単な日本語訳のようなものです。
* [ilyavorobiev/atom-docs](https://github.com/ilyavorobiev/atom-docs) - Atom-shellの構造について書かれたドキュメントです。

## 類似ツール

Electronと同じように以下のソフトウェアを使うことで、クロスプラットフォーム向けのデスクトップアプリケーションを作ることができます。ただ、Electronとまったく同じではありませんので作りたいものに応じて使い分けてください。

* [quark-shell-mac](https://github.com/HackPlan/quark-shell-mac)
* [node-webkit](https://github.com/nwjs/nw.js)
* [MacGap](https://github.com/MacGapProject/MacGap1)




## その他

### ドキュメントの翻訳方法

`atom/electron.atom.io`で`atom/electron/docs`内の日本語翻訳については「[Translation in Japanese #20](https://github.com/atom/electron.atom.io/issues/20)」で翻訳する手順は以下のようになっております。興味がある方はぜひ参加してください。

また、今後誰もが簡単に翻訳ができるようにガイドラインの作成についても「[Create a guide for translation #28](https://github.com/atom/electron.atom.io/issues/28)」で話し合っています。

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

## タスク

* [ ] 各ソフトウェアを比較した表作成
* [ ] コントリビュートファイル作成
* [ ] 英語版作成

## コントリビュート

このドキュメントの分かりにくい部分や質問がある際は、`README.md`内の該当箇所をコピーしてください。その後その文とともにissueを作成してください。気軽にissueを作成していただければ幸いです。

例：

```
> Electronはクロスプラットフォームアプリケーションシェル...

Electronとは何ですか？
```

## ライセンス

MIT © Sota Yamashita
