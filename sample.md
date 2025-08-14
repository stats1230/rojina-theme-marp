---
marp: true
theme: rojina
paginate: true
lang: ja
footer: '<div>氏名</div><div>報告タイトル</div>'
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

### 日付 | 報告の場所
# 報告タイトル
## 報告サブタイトル


<div class="author-block" markdown="1">

### あなたの名前
あなたの所属
あなたの email、twitter、github、etc...

</div>

---
<!--
_header: '**太字にすると濃くなって**、それ以外はちょっと薄いよ'
-->
## ページの見出し

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

## 適当なタイトル
- 行の途中に `code` を追加できる
- バックティック "```" で囲むと、長いコードブロック

```
library(tidyverse)
library(estimatr)

df <- read_csv('data/hoge.csv')
```

  <div class="block">
    <div class="block-title">タイトル</div>
    <div class="block-content">本文</div>
  </div>

---
<!--
_header: 'ヘッダも書けるよ'
-->

## 参考文献

<div class="ref">
  <p>
  ll
  </p>
</div>

Anderson, J. R., & White, E. M. (2024). The psychological impact of imaginary numbers on abstract thought. Journal of Fictional Psychology, 10(3), 112-125.

Chen, L. F. (2023). A new species of flying fish discovered in a non-existent ocean. Annals of Hypothetical Zoology, 5(1), 45-58.

Davis, S. L., & Green, M. T. (2022). The spectral properties of invisible light. Quantum Nonsense Review, 21(4), 301-315.

Evans, P. R. (2021). Chronological inconsistencies in time-travel narratives. Journal of Temporal Studies, 7(2), 88-102.

Foster, G. H., & Hall, R. L. (2020). The sociological implications of a society with no gravity. Journal of Gravitational Sociology, 14(3), 205-220.

Garcia, D. M. (2019). The linguistic structure of a language spoken only in dreams. Phantasmagorical Linguistics, 3(1), 1-15.

Harris, A. J., & Miller, B. K. (2018). The culinary history of forgotten foods from a parallel universe. Historical Gastronomy Quarterly, 11(2), 65-79.

Johnson, L. S. (2017). The geological formation of floating islands. Journal of Earth-Like Planets, 6(4), 150-162.

Kim, Y. S. (2024). The Encyclopedia of Imaginary Creatures. Fictitious Press.

Lopez, F. D. (2023). A Comprehensive Guide to Non-Existent Technologies. Unreal Publishing.

Martinez, E. R. (2022). Advanced Calculus for Impossible Shapes. Paradoxical University Press.

Nelson, O. B. (2021). Metaphysics of the Unseen. Shadow Books.

Patel, R. N. (2020). The Secret History of the World that Wasn't. Mythos Publishing.

Quinn, W. F. (2019). The Art of Drawing Nothing. Empty Canvas Books.
</p>
</div>