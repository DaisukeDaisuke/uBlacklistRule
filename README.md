# uBlacklistRule

[uBlacklist](https://iorate.github.io/ublacklist/)向けのルールです。

# 購読

こちらから最新版の購読が可能です。

<https://raw.githubusercontent.com/ncaq/uBlacklistRule/master/uBlacklist.txt>

# 何故既にルールを共有するリポジトリがあるのに新しく作ったのか

[arosh/ublacklist-stackoverflow-translation: Stack Overflow の機械翻訳サイトの除外用フィルタ](https://github.com/arosh/ublacklist-stackoverflow-translation)
など、
すばらしい先駆者様が居ます。

ただ、
このリポジトリの対象はあくまで機械翻訳サイトのみなので、
もっと広くブロックする自前のルールを作っていました。

メンテナンスが結構大変になってきたので、
生成ツール付きで独立リポジトリとして公開することにしました。

# ブロックするサイト

## 技術系スパムサイト

[Stack Overflow](https://stackoverflow.com/)などから機械翻訳した内容を大量生成するサイトです。

翻訳してないで単にコピーしているサイトも入ってることがあります。

## コピペサイト

特に新しい情報を生み出さないスパムサイト。
いわゆるデッドコピーです。
webプロキシなども対象です。
webプロキシを使いたい場合普通検索結果経由では行きませんよね?

## 5chのコピーサイト

[５ちゃんねる](https://5ch.net/)などから内容をコピーした、
**機械生成の割合が高い**サイトです。

### 全てをブロックしない理由

一つは、
あまりにもサイト数が多いので対処しきれないためです。

もう一つは、
5chは条件付きでまとめサイトの生成を許可しているためです。
[5chまとめブログ・5chまとめアプリ運営者の皆さまへ](https://5ch.net/matome.html)

## YouTube、ニコニコ動画などのコピーサイト

インラインで動画を出していたりメタデータを転載しているサイトです。

## コピーゲーム攻略サイト

他の情報源からゲームの攻略情報をコピーしていたり、
「工事中」でページを埋めたりする、
いわゆる企業型攻略サイトです。

## デマサイト

主にゲハブログなど悪質なデマを撒き散らすサイトです。

## その他検索の役に立たないサイト

要らない検索結果はガンガン排除していきます。

# 存在しないサイトのURLがたくさん載っている理由

コピーサイトはドメインの一部分を変えるなどの方法でどんどん増えていきます。
増えるたびにリストに追加するのは面倒です。
機械増殖には機械増殖で対応します。
よってこちらもURLを自動生成します。

# このサイトが載ってないのはおかしい/このサイトが載っているのはおかしい

Issue, Pull Requestを是非ともお待ちしております。

Issueだけ建てるのも歓迎しますし、
[uBlacklistRule/Host.hs at master · ncaq/uBlacklistRule](https://github.com/ncaq/uBlacklistRule/blob/master/src/Host.hs)
などに書き込んでくださるのも歓迎いたします。

# 関連リンク

* [uBlacklistを使ってポケモン徹底攻略やStack OverflowのコピペサイトをGoogle検索から除外しましょう - ncaq](https://www.ncaq.net/2019/12/18/19/18/05/)
* [uBlacklist - iorate.github.io](https://iorate.github.io/ublacklist/)
* [iorate/uBlacklist: Blocks specific sites from appearing in Google search results](https://github.com/iorate/uBlacklist)
* [アフィカスリスト作成所 - なんJ AdGuard部 Wiki*](https://wikiwiki.jp/nanj-adguard/%E3%82%A2%E3%83%95%E3%82%A3%E3%82%AB%E3%82%B9%E3%83%AA%E3%82%B9%E3%83%88%E4%BD%9C%E6%88%90%E6%89%80)
