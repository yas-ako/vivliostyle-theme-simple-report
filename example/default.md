---
title: 'Vivliostyle Theme Exampleaaa'
body:
  class: 'chapter1'
vfm:
  hardLineBreaks: false
---


# Vivliostyle Simple Report Theme


<div class="author">

- 著者の名前1
- 著者の名前2

</div>

このテーマは、Vivliostyle を使用してシンプルなレポートを書くためのテーマです。
Vivliostyle Flavored Markdown（VFM）を使用することで、Markdown 形式で書かれた原稿をを PDF などの形式に変換できます。

公式テーマである[Academic](https://github.com/vivliostyle/themes/tree/main/packages/%40vivliostyle/theme-academic) を参考に、いくつかの機能を追加してあります。


## テーマの使い方

(加筆予定)

## 機能の一覧

### 表紙ページ

この機能は、Academic テーマの実装をほとんどそのまま使用しています。

`.cover` クラスを持つ `div` 要素で囲むことで、表紙ページを作成できます。
`.cover` クラス内の `h1` 要素がレポートのタイトルとなり、`.author` クラス内の `ul` 要素が著者名のリストとなります。

```markdown
<div class="cover">

# Vivliostyle Simple Report Theme

<div class="author">

- 著者名1
- 著者名2

</div>
</div>
```

## ソースコード

### シンタックスハイライト

```javascript
function main() {}
```

````
```javascript
function main() {}
```
````

### キャプションを付与

```javascript:app.js
function main() {}
```
````
```javascript:app.js
function main() {}
```
````
または、次のようにしてもよい
````
```javascript title=app.js
function main() {}
```
````

## 数式の挿入

<div class="math">

$$ax^2+bx+x=0$$

</div>

<div class="math">

$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$

</div>

## 図表の挿入・参照

<div class="math">

$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$

</div>


<div class="math">

$$x=\frac{-b\pm\sqrt{b^2-4ac}}{2a}$$

</div>


---

## 箱

- 箱で囲むことができます。
- `.box` クラスを指定します。
- 箱の見た目や役割を変更したい場合は、次のいずれかの値を追加してください。
  - `.example` - 例題
  - `.theorem` - 定理
  - `.proof` - 証明
- `.box` 要素内の先頭や最後にある要素の余白を削ります。
- 要素内の先頭に`**微積分学の基本定理**`などと書くと、その行が見出しとなり、自動で番号が挿入されます。

```markdown
<div class="box" data-box-type="example">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>
```

---


### 例題

- 見出しが枠線の上にある枠を生成します。

<div class="box" data-box-type="example">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>


<div class="box" data-box-type="example">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>


<div class="box" data-box-type="example">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

<div class="box" data-box-type="example">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

### 定理

- 背景が灰色の枠を生成します。

<div class="box" data-box-type="theorem">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

<div class="box" data-box-type="theorem">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

<div class="box" data-box-type="theorem">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

### 証明

- 左の枠線のみがついた枠を生成します。

<div class="box" data-box-type="proof">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>


<div class="box" data-box-type="proof">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

<div class="box" data-box-type="proof">

**微積分学の基本定理**

微積分学の基本定理は、微分と積分の関係を示す定理です。

</div>

---

## 引用

### 脚注

章の最後にまとめて脚注を挿入できます。

VFM is developed in the GitHub repository[^1].
Issues are managed on GitHub[^issues].
Footnotes can also be written inline^[This part is a footnote.].

[^1]: [VFM](https://github.com/vivliostyle/vfm)
[^issues]: [Issues](https://github.com/vivliostyle/vfm/issues)

### 傍注

注釈を付与したい内容のあるページの余白に注釈を表示します。

## Frontmater

(You can define metadata on the top of the Markdown file. Try to set `lang` option `ja` in the frontmatter! If you need more information, please check [Frontmatter part in VFM document](https://vivliostyle.github.io/vfm/vfm#frontmatter).)

## Hard new line

(Try to set the `hardLineBreaks` option `true` in the frontmatter!)

はじめまして。

Vivliostyle Flavored Markdown（略して VFM）の世界へようこそ。
VFM は出版物の執筆に適した Markdown 方言であり、Vivliostyle プロジェクトのために策定・実装されました。

## Image

![](<./assets/Logo%20(Mark%20+%20Type).png>)

### with caption and single line

![Vivliostyle Logo](<./assets/Logo%20(Mark%20+%20Type).png>)

![Vivliostyle Logo](<./assets/Logo%20(Mark%20+%20Type).png> 'distributed on the official website'){id="image" data-sample="sample"}

text ![Vivliostyle Logo](<./assets/Logo%20(Mark%20+%20Type).png>)

## Math equation

<!-- inline: $x = y$ -->

<!-- display: $$1 + 1 = 2$$ -->

## Raw HTML

<div class="custom">
  <p>Hey</p>
</div>

### with Markdown

<div class="custom">

- hoge
- fuga

</div>

## Ruby

This is {Ruby|ルビ}

### Escape pipe in ruby body

{a\|b|c}

## Sectionization

## Plain ##

## Introduction {#intro}

## Welcome {.title}

## Level 1

### Level 2

> ## Not Sectionize

---
---