---
hide:
  - navigation
  - toc
---

# ウェブハンドリング技術解説

ロールトゥロール（R2R）搬送 — フィルム・紙・金属箔などの **薄物連続材料を破らず・しわを作らず・蛇行させず・きれいに巻く** ための技術を、現場の製造・保全エンジニア向けに体系的に解説するサイトです。

[基礎から読む :material-arrow-right:](basics/overview.md){ .md-button .md-button--primary }
[用語集を見る :material-book-open-variant:](basics/glossary.md){ .md-button }

---

## このサイトの特徴

<div class="grid cards" markdown>

-   :material-book-multiple:{ .lg .middle } **書籍ベースの体系的解説**

    ---

    橋本『入門ウェブハンドリング』『ウェブハンドリングの基礎理論と応用』、『スリッター・リワインダーの技術読本』、『実践ウェブハンドリング』など主要4冊の理論を整理。章節レベルで参照可能。

-   :material-calculator-variant:{ .lg .middle } **数式と図で理解**

    ---

    オイラーの摩擦式、Hakiel 巻取理論、ウェブの直角方向進入性など、核心理論を MathJax 数式と Mermaid 図で平易に解説。

-   :material-tools:{ .lg .middle } **実務直結のトラブル対応**

    ---

    しわ・蛇行・テンション変動・テレスコープ等、現場で頻発するトラブルの原因切り分けと対策を整理。

-   :material-school:{ .lg .middle } **読者対象**

    ---

    ウェブハンドリングに関わる製造・保全・設計エンジニア、新人技術者の入門、現場リーダーの再学習に。

</div>

---

## 主要カテゴリ

<div class="grid cards" markdown>

-   :material-book-open-page-variant:{ .lg .middle } **[基礎知識](basics/overview.md)**

    ---

    ウェブハンドリングとは／用語・記号一覧／フィルム・紙・金属箔の材料特性

-   :material-gauge:{ .lg .middle } **[テンション制御](tension/theory.md)**

    ---

    張力の基本理論／オイラーの摩擦式／テンション分布／制御機器の選定

-   :material-circle-slice-6:{ .lg .middle } **[ロール・搬送系の力学](roll/mechanics.md)**

    ---

    ロール周りの力学（Hakiel理論）／ニップ／駆動系／マイクログルーブローラ

-   :material-swap-horizontal:{ .lg .middle } **[蛇行制御](steering/mechanism.md)**

    ---

    蛇行の発生メカニズム／ガイドロールの設計／EPC等の自動蛇行修正装置

-   :material-alert-circle:{ .lg .middle } **[トラブルシューティング](trouble/wrinkle.md)**

    ---

    しわの原因と対策／テンション変動の対策／蛇行トラブルの対策

</div>

---

## 代表的な公式

ウェブハンドリングの設計を支配する最重要式の一つが、**オイラーのベルト摩擦式**：

$$
\frac{T_2}{T_1} \le e^{\mu \theta}
$$

ここで $T_1, T_2$ はロール前後の張力、$\mu$ はウェブ・ロール間の摩擦係数、$\theta$ は巻き付き角（ラジアン）。
高速搬送ではこの関係が成立しなくなり、スリップ・蛇行・しわが連鎖的に発生します。詳細は [オイラーの摩擦式](tension/euler.md) を参照。

---

## はじめての方へ

!!! tip "おすすめの読み順"
    1. [ウェブハンドリングとは](basics/overview.md) — 全体像と本サイトの構成
    2. [用語・記号一覧](basics/glossary.md) — 主要用語を押さえる
    3. [テンション制御の基本理論](tension/theory.md) — もっとも重要な「張力」の物理
    4. 興味のあるカテゴリに進む

!!! info "本サイトについて"
    本サイトは MkDocs Material で構築され、[GitHub](https://github.com/hajime-tech/web-handling) でソースを公開しています。
    記述の誤りや改善提案は GitHub Issue にてお寄せください。

!!! warning "免責"
    本サイトの内容は技術理解の助けを目的とした解説であり、実機の設計・運用判断は必ず一次資料（書籍・メーカ仕様書）と現場検証に基づいて行ってください。
