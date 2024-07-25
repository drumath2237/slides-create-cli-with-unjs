---
# You can also start simply with 'default'
theme: default
title: UnJSを使って軽率にCLIを作ってみたらめちゃくちゃ便利だった
info: v-tokyo 21でのLT登壇資料
author: にー兄さん
class: text-left
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
# transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
colorSchema: dark
mdc: true
fonts:
  sans: M PLUS 2
  mono: JetBrains Mono
layout: intro
hideInToc: true
download: true
export:
  dark: true
exportFilename: create-cli-with-unjs
---

# UnJSを使って[軽率に]{style="color:#33CCFF"}
# CLIを作ってみたら
# めちゃくちゃ便利だった

### にー兄さん[@ninisan_drumath](https://twitter.com/ninisan_drumath)  
### v-tokyo #21

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

- 個人開発しているCLIでUnJSを使ってみた
- どんなパッケージを使ったのか、用途別にご紹介
- UnJSのパッケージが気になっている方に刺さると嬉しいです

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

<img src="/run2.png" class="ml-10 mb-10" />
<img src="/run-web.png" class="ml-10" />

---
level: 2
---

# create-babylon-appの要件

1. 作成するプロジェクト名を指定
2. テンプレートを選択
3. 設定を反映したプロジェクトを作成

create-viteやNuxt CLIの動作に近いので参考にしている。

---
level: 2
---

# UnJSとは

> UnJSは、Nuxt 開発チームが中心となって開発・メンテナンスされている、あらゆるJavaScriptフレームワーク上で統一的に動作するユーティリティーツール・ライブラリ群です。[^1]

[^1]:『[UnJS にどんなツールがあるのか、上位30件すべて紹介してみた（前編）](https://zenn.dev/ytr0903/articles/c6c42147ed29be)』より

---
level: 2
layout: two-cols
---

# UnJSを使ってみたい
<br/>

便利なパッケージがたくさんあるんだなぁ

自分でメンテしているCLIに使えないかな......？

<style>
.footnote-item p{
  font-size: 1rem
}
</style>

::right::

GANGANさんのツイートを発見

<Tweet id="1744908147733692742" scale="0.65" class="ml-10"/>

---
layout: section
---

# 使用したUnJSパッケージ

---
level: 2
---

# 使用したパッケージ一覧

- unbuild
- citty
- jiti
- consola
- giget
- pkg-types

---
level: 2
---

# <twemoji-package /> unbuild

> A unified javascript build system

https://unjs.io/packages/unbuild


---
level: 2
---

# <twemoji-cityscape-at-dusk /> citty

> Elegant CLI Builder

https://unjs.io/packages/citty

---
level: 2
---

# <twemoji-koala /> consola

> Elegant Console Wrapper

https://unjs.io/packages/consola

---
level: 2
---

# <twemoji-french-fries /> jiti

---
level: 2
---

# <twemoji-sparkles/> giget

---
level: 2
---

# <twemoji-beverage-box/> pkg-types

---
layout: section
---

# おわりに

---
level: 2
---

# まとめ

---
level: 2
---

# 参考文献
