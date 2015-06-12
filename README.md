Documentation for Electron
==========================

_Note: This document is written in Japanese. It will be English_

TL;DR

>Electron is the cross-platform application shell we originally built for the Atom editor to handle the Chromium/Node.js event loop integration and native APIs.

Electronはクロスプラットフォームアプリケーションシェル。もともとはChromium/Node.jsのevent loop integrationやネイティブAPIをAtomエディタで使うために作られました。

--

Atom-shellの設計について書かれた[ilyavorobiev/atom-docs](https://github.com/ilyavorobiev/atom-docs)というドキュメンがありました。しかし現在メンテがされていないので一部情報の修正と追加、その翻訳も含めてドキュメントを作成することにしました。

Electronについて勉強はしていますがすべてを知っているわけではありません。もし何かありましたらコントリビュートを参考にissueを作成していただくか、Twitterを[@sota0805](https://twitter.com/sota0805)でやっているのでコメントを頂ければと思います。

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
 * コントリビュート
* タスク
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

## コントリビュート

このドキュメントの分かりにくい部分や質問がある際は、`README.md`内の該当箇所をコピーしてください。その後その文とともにissueを作成してください。気軽にissueを作成していただければ幸いです。

例：

```
> Electronはクロスプラットフォームアプリケーションシェル...

Electronとは何ですか？
```

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Electron docs</span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.com/sotayamashita/electron-docs" property="cc:attributionName" rel="cc:attributionURL">Sota Yamashita</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc/4.0/">Creative Commons Attribution-NonCommercial 4.0 International License</a>.
