# Rojina: Marp Theme
"Rojina" は、特に政治学系の学術報告スライドのために作成されたカスタムテーマです。デザインと機能の両方でモダンでプロフェッショナルなテーマを目指しています。

## Marp
このテーマは、Marp 向けに作られています。Marp の使い方などは[公式ドキュメント](https://marp.app/)などを参照してください。


## 使い方

Marp for VS Code または Marp CLI のいずれかの環境が前提です。後者を使う人には説明は不要でしょうから、下記は VS Code で使う人向けの手順です。

#### 1. CSS ファイルを配置する
- `marp-theme/rojina.css` をダウンロードし、適当な場所に配置します。
  - おすすめは、作業ディレクトリに `marp-theme` というディレクトリを作成することです。
  - Settings > Marp: Themes にパスを記入します。
- または、Settings > Marp: Themes に次のように入力します。
  - `https://stats1230/rojina-theme-marp/`

#### 2. Yaml ヘッダの指定
- sample.md を参考に、Markdown ファイル (`.md`) を作成します。
- Markdown ファイルの先頭にある yaml ヘッダに、次のように記述します。

```yaml
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
```

- それ以降は、通常の marp の方法に従ってファイルに記入していきます
- このテーマの独自の機能などについては、sample.md 及び後述の「Rojina の推しポイント」をご覧ください。


#### 3. PDF への出力
- コマンドパレット (VS Code の画面上部) から `Export Slide Deck` を選択します
  - PDF への出力は Chrome系のブラウザが必要になります。

## Rojina の推しポイント
ここからは、Rojina テーマに実装したいくつかの機能をまとめます。

### 