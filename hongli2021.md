---
id: "hongli2021"
aliases:
  - "HongLi2021"
  - "Universal Representation Learning from Multiple Domains for Few-shot Classification"
tags:
  - "paper"
---

# Universal Representation Learning from Multiple Domains for Few-shot Classification

## 背景・目的

学習データに現れないドメインに対して、一般化する手法に関心が移っってきている。（現実的な設定であるため）
そこで、複数ドメインにおいて効率的かつパフォーマンスの良い手法を提案した。

## 関連研究との違いは？

関連研究は興味ない

## 提案：解決に向けたキーアイデア

知識蒸留を用いて、ドメイン毎の汎用的な知識を学習している。
蒸留をする際に、ドメイン固有の特徴量を抽出するモデルと、分類を行う分類器を用いて学習を行う。

## 結果:結局問題は解決されたのか．新しくわかったことは？

既存手法よりもよい制度を達成した。
また、学習データに現れていないドメインについても、既存手法よりも良い精度を達成することができた。

