---
id: "verma2022"
aliases:
  - "verma2022"
  - "Calibrated Learning to Defer with One-vs-All Classifiers"
tags:
  - "paper"
  - "Human-AI"
---
# Calibrated Learning to Defer with One-vs-All Classifiers

## 背景・目的

L2Dフレームワークにおいて、[[mozanner2020]]らの手法の問題点を指摘した。
その問題点を改善したOne-vs-Allベースの損失関数を提案している。

## 関連研究との違いは？

[[mozannar2020]]らの手法は[[madras2018]]らの手法をベースにしたSofmatxベースの手法を提案した。
[[raghu2019]]では、信頼度ベースの手法の制約についての研究が行われている。

この論文では、L2Dフレームワークにおいて、より良い後処理の手法を初めて提案している。

## 提案：解決に向けたキーアイデア

[[mozanner2020|Mozanner2020]]らの手法では、人間の予測の正解確率を推定しているがこの推定値の後処理が不十分であることを示した。

この不十分さを解決するために、OvAベースの損失関数を提案した。
分類関数とrejection関数の定義は[[mozannar2020]]と同じ。
\phiは何らかのバイナリ損失関数。

!()[./img/verma2022_loss.png]

## 結果:結局問題は解決されたのか．新しくわかったことは？

[[mozannar2020]]、[[okati2021]]の手法と比較したところ、良い精度を達成することができた。

!()[./img/verma2022_result.png]


## 感想

softmaxベースの手法の悪い点がわかっていないが凄そうではある
