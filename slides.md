---
# You can also start simply with 'default'
theme: default
title: |
  create-babylon-appを
  軽率にアプデしたい
info: Babylon.jsゆるほめLT会 vol.3での発表資料
author: にー兄さん@drumath2237
class: text-left
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
# transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
fonts:
  sans: M PLUS 2
  mono: JetBrains Mono
layout: intro
hideInToc: true
download: true
export:
  dark: true
exportFilename: update-create-babylon-app-slide
---

# create-babylon-appを
# [軽率に]{style="color:#33CCFF"}アプデしたい

### にー兄さん[@ninisan_drumath](https://twitter.com/ninisan_drumath)  
### Babylon.js ゆるほめLT会 vol.3

---
layout: two-cols
hideInToc: true
---

# にー兄さん

- ソフトウェアエンジニア@HoloLab inc.
- Babylon.js勉強会運営
- Iwaken Lab.

好きなもの

- Babylon.js / WebXR Device API / C#
- ねこ / コーヒー / ウィスキー / ギター

アカウント

- <uim-twitter-alt /> [@ninisan_drumath](https://x.com/ninisan_drumath)
- <uim-github-alt /> [@drumath2237](https:github.com/drumath2237)

::right::

<img src="https://pbs.twimg.com/profile_images/1113849253548269568/4uy_K_LA_400x400.png" class="rounded shadow m-30 h-60"/>

---
hideInToc: true
---

# 本日の話

- create-babylon-appの開発進捗について共有
- Babylon.jsの話はほぼ出てきません（おい）

---
hideInToc: true
---

# アジェンダ

<Toc maxDepth="1"/>

---
layout: section
---

# はじめに

---
level: 2
layout: two-cols
---

# create-babylon-app とは

- Babylon.jsのプロジェクトを簡単に作成するためのCLI
- コマンドラインから質問に答えるとプロジェクトができ、そのまま開発できる手軽さが売り

お手元のターミナルでぜひ試してみてください！<twemoji-backhand-index-pointing-down />

```txt
npm create babylon-app
```

GitHub: https://github.com/drumath2237/create-babylon-app

<style>
code.language-txt{
  font-size: 1.2rem
}
</style>

::right::

<img src="/run.png" class="m-10" />
<img src="/run-web.png" class="m-10" />

---
level: 2
layout: two-cols
---

<Tweet id="1676571182483800064" scale="0.75" />

::right::

実は去年のゆるほめLTでも  
発表していました。

---
level: 2
layout: center
---

# たまにフォーラムに反応があった

<img src="/forum-reac.png" class="size-3/4">

---
level: 2
layout: two-cols-header
---

# もしかしたら公式docsに載せて......もらえなかった

::left::

<img src="/docss.png" class="w-5/6">

::right::

公式docsに載ってるViteのサンプルが普通ではないフォルダ構造になっていて混乱したらしい。

公式の内容をこちらに置き換えないか？というポスト

「正直なところこのツールは完璧とは程遠い」

惜しい...！

---
level: 2
---

# ちゃんとメンテしよう

- ある程度需要はある気がしてきた
- ちゃんと作れば公式ツールになっちゃうかも！？
- えいやとリリースしてからアプデできていなかった

これらにより、開発のモチベが上がってきた

---
layout: section
---

# アプデの進捗と目標

---
level: 2
layout: two-cols
---

# ｖ0.1.7のリリース

- 依存パッケージのアプデ
- Linter/FormatterをBiomeへ移行
- CI/CDの改善

などを行い、v0.1.7を先日リリース<twemoji-party-popper />

これにより作成できるプロジェクトがBabylon.js 7に対応したりした

::right::

<Tweet id="1809238774771273919" scale="0.65" />

---
level: 2
---

# Road to v1.0.0
<br/>
GitHub ProjectsのKanban上でタスク管理

<img src="/kanban.png" />

---
level: 2
---

# 対応したい項目たち

1. より便利なテンプレートの追加
2. UnJSパッケージへの移行
3. コマンドライン引数の対応
4. ドキュメントページの作成

---
level: 3
layout: two-cols
---

## テンプレートの追加
<br/>

現状はPlayground準拠のTypeScript・JavaScript用テンプレしかない

希望としては下記ラインナップにしたい

- シンプルなテンプレート
- Playground準拠テンプレート
- Babylon.jsライブラリ開発テンプレート
- コミュニティ提供テンプレート群
  - WebXR用とかReact用とか...

::right::

## UnJSパッケージへの移行

UnJSから提供されているCLI作成に便利なパッケージ群に移行したい

- citty
- consola
- jiti
- giget
- unbuild

<img src="https://unjs.io/favicon.svg" class="mt-10 w-[8rem]" />

---
layout: section
---

# おわりに

---
level: 2
---

# おわりに

- create-babylon-appをちゃんとメンテします（宣言）
  - 色んな人に便利に使ってもらえるような状況へ
- 7月末～8月上旬くらいに1.0リリースを目標に

---
level: 2
---

# 関連・参考

- create-babylon-app（GitHub）  
https://github.com/drumath2237/create-babylon-app
- Kanban（GitHub Projects）  
https://github.com/users/drumath2237/projects/13
- create-babylon-app　v1.0に向けたアプデ作業（Zenn）  
https://zenn.dev/drumath2237/scraps/b085d5f90b65f3