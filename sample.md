---
marp: true
theme: rojina
paginate: true
lang: ja
footer: '<div>達野俊輔</div><div>Rojina: Marp で研究報告</div>'
style: |
  section {  
    --prim-color: #03233aff;      /* プライマリカラー */
    --sec-color: #2a4f69ff;       /* セカンダリカラー */
    --color-background: #fdfdfd;  /* 背景の色 */
    --color-foreground: #333;     /* 文字の色 */
    --color-link: var(--sec-color); /* リンクの色 */
    }
---
<!--
_class: title-page
_paginate: false
_footer: ''
-->

### 2025年9月25日更新 | 研究室の机
# Rojina: Marp で研究報告
## 政治学系の研究報告に使えそうな Marp 用の <br>カスタム CSS を作ってみた


<div class="author-block" markdown="1">

### 達野俊輔
一橋大学大学院法学研究科
E-mail: jm240007@hit-u.ac.jp, Twitter: [S1230Tats](https://x.com/S1230Tats)

</div>

---
<!--
_header: 'ページごとにヘッダーを書くことができます'
-->
## Marp : 研究報告スライドに使えそう
- Marp とは、Markdown 記法でスライドがかけるシステム
  - 公式ドキュメントは[こちら](https://marp.app/)
- Markdown, HTML, CSS を適用することができる

### 研究報告のスライド、頑張って作りたくない
- スライドのデザインって、結構面倒。
  - ゼミや勉強会のたびにスライドを作成し、その都度デザインを考えたくない！
  - パワポとか Google Slides は親切な機能が多すぎ！
  - 内容を考えることに集中したい！

▷ **研究報告に特化した Marp のテーマ作っちゃった！**

---
<!--
_header: 'ページごとにヘッダーを書くことができます'
-->
## Marp : 研究報告スライドに使えそう
### Marp はこんな人におすすめ
- できる限り低コストでスライドを作りたい (時間も脳のリソースも)
  - 文字サイズとかフォントとか、いちいち設定している時間って必要？
  - 普段書いている Markdown のメモからスライド作りたい
- パワポや Slides の余計な機能から解放されたい
- スライド内に数式を含めたい
  - ~~なんかパワポは数式に対応してるっぽいやん~~
- もっと気になるなら、その他の布教記事も読んでみて
  - [Markdown でスライドを作れる Marp はいいぞ](https://qiita.com/tomoasleep/items/604107787d92dec4868e)
  - [Marpで研究発表スライドを作る 〜Beamerを卒業しよう〜](https://zenn.dev/hellorusk/articles/4edf3920dd1a35)
  - [Marpで作るゼミ資料 〜CSS例を添えて〜](https://qiita.com/NAT/items/6f7fc309849f0c30992f)

---
<!--
_header: '**太字にすると**、ちょっとだけ色が濃くなります'
-->

## Marp : はじめて使う人へ
- Marp 全般に関しては、前頁の記事や[公式ページ](https://marp.app/)を読んでください
- Markdown 記法の知識が必要です。下記の記事が詳しいです。
  - [Markdown記法 チートシート](https://qiita.com/Qiita/items/c686397e4a0f4f11683d)
  - 基本的には習うより慣れろ、です。
- 数学を使うときは  $\TeX$ の知識が必要です。
  - みんな大好き [TeX Wiki](https://texwiki.texjp.org/)

- VS Code で作成するのがおすすめです
  - 拡張機能として、以下が便利です。
  - Marp for VS Code (必須)、Markdown All in One (推奨)

---
<!--
_header: '**Rojina の使い方**'
-->

## Rojina : 本文のスタイル
### 見出し3は、太字の見出しです
具体的な使い方の説明は GitHub やブログに任せるとして、ここでは Rojina テーマのサンプルを提示します。

#### 見出し4は、ちょっと太いです。
- 箇条書きは簡単に使えて、
  - レベルが深くなると文字が
    - どんどん小さく
      - なっていきます (こんなに深い箇条書きはあまり使わないほうがいいよ)
1. 数字付きの箇条書きも同様に書けます
2. 拡張機能を使うと、勝手に番号を振ってくれるので便利です。

---
<!--
_header: '**Rojina の使い方**'
-->
## Rojina : 本文のスタイル
### 脚注を使うことができる

LaTeX と Markdown の機能を利用 (悪用？) して$^1$、脚注を再現しています。

- 「スライドで脚注を使うことがあるか」というコメントは受け付けません。
  - 個人的には、脚注に文献情報 (著者年)  を書くことが多いです$^4$

> 1: $\LaTeX$ の右上付き添字と、Markdown の引用の機能を使っています。
> 2: 本当の脚注じゃないので、任意の脚注を勝手に追加することができます。
> ア: もちろん、脚注番号も適当に振ることができます。
> 4: Wilds (2099)

---
<!--
_header: '**Rojina の使い方**'
-->
## Rojina : 本文のスタイル
### 表を挿入する
- 表を挿入することも可能です (次頁を参照)。
- Markdown 記法のシンプルな表のみ対応しています。


### テーマカラーを変更する
- yaml ヘッダのカラーコードを指定することで、スライドのテーマカラーを変更できます
- 各カラーの変数は次頁の表のとおりです


---
<!--
_header: '**Rojina の使い方**'
-->
## Rojina : 設定できるテーマカラー

| 変数名 | 概要 |
| :--- | :--- |
| --prim-color | メインのカラー。ページタイトルの背景色や、 ボックスの見出し色に使われています。|
| --sec-color | サブのカラー。コードの背景とフッタに使われています。メインカラーと同系統の色がおすすめ。 |
| --color-background | 全体の背景の色です。ページタイトルの文字色にも使われています。 |
| --color-foreground | 文字の色です。 |
| --color-link | リンクを張った際の文字と下線の色です。デフォルトでは --sec-color がそのまま使われています。 |


---
<!--
_header: '**太字にすると濃くなって**、それ以外はちょっと薄いよ'
-->

## Rojina : コードを挿入する
### インライン・コード
- 1つのバックティック ("`") で囲むと行の途中にコードかける
  - 重回帰分析は `estimatr::lm_robust()` がいいよ
  
### コードブロック
- 3つのバックティック "```" で囲むと、長いコードブロック

```
library(tidyverse)
library(estimatr)

df    <- read_csv('data/hoge.csv')
model <- lm_robust(y ~ are + kore + sore, data = df)
```

---
<!--
_header: '**太字にすると濃くなって**、それ以外はちょっと薄いよ'
-->

## Rojina : 数式を挿入する
### インライン数式
- 1つのドル ("$") で囲むと行の途中に数式が書ける
  - 変数 $X_k$ の偏回帰係数 $\beta_k$ は、限界効果などと呼ばれる
  
### コードブロック
- 2つのドル "$$" で囲むと、長い数式ブロック

$$
E[Y | \boldsymbol{X}] = \beta_0 + \beta_1 X_1 + \cdots + \beta_M X_M
$$

$$

E[X] = \left\{
\begin{array}{ll}
\int_{-\infty}^\infty tf(t)dt & (X が連続変数)\\
\sum_{i = 1}^{n}x_ip(x_i) & (X が離散変数)
\end{array}
\right.$$

---
<!--
_header: 'ヘッダも書けるよ'
_class: ref
-->

## 参考文献


Anderson, J. R., & White, E. M. (2024). The psychological impact of imaginary numbers on abstract thought. _Journal of Fictional Psychology, 10_(3), 112-125.

Chen, L. F. (2023). _A new species of flying fish discovered in a non-existent ocean. _Annals of Hypothetical Zoology, 5_(1), 45-58.

Davis, S. L., & Green, M. T. (2022). _The spectral properties of invisible light. _Quantum Nonsense Review, 21_(4), 301-315.

Evans, P. R. (2021). _Chronological inconsistencies in time-travel narratives. _Journal of Temporal Studies, 7_(2), 88-102.

Foster, G. H., & Hall, R. L. (2020). The sociological implications of a society with no gravity. _Journal of Gravitational Sociology, 14_(3), 205-220.

Garcia, D. M. (2019). _The linguistic structure of a language spoken only in dreams. _Phantasmagorical Linguistics, _3(1), 1-15.

Harris, A. J., & Miller, B. K. (2018). The culinary history of forgotten foods from a parallel universe. _Historical Gastronomy Quarterly, 11_(2), 65-79.

---
<!--
_header: 'ヘッダ書かなくてもいいんだけどね'
_class: ref
-->

## 参考文献

Johnson, L. S. (2017). The geological formation of floating islands. _Journal of Earth-Like Planets, 6_(4), 150-162.

Kim, Y. S. (2024). _The Encyclopedia of Imaginary Creatures_. Fictitious Press.

Lopez, F. D. (2023). _A Comprehensive Guide to Non-Existent Technologies_. Unreal Publishing.

Martinez, E. R. (2022). _Advanced Calculus for Impossible Shapes_. Paradoxical University Press.

Nelson, O. B. (2021). _Metaphysics of the Unseen_. Shadow Books.

Patel, R. N. (2020). _The Secret History of the World that Wasn't_. Mythos Publishing.

Quinn, W. F. (2019). _The Art of Drawing Nothing_. Empty Canvas Books.

