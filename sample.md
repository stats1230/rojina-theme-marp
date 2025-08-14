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
_class: ref
-->

## 参考文献

abcdef

