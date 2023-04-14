---
id: "wallace2019"
aliases:
  - "wallace2019"
  - "Trick Me If You Can: Human-in-the-Loop Generation of Adversarial Examples for Question Answering"
tags:
  - "paper"
  - "annotation_support"
  - "QA"
---
# Trick Me If You Can: Human-in-the-Loop Generation of Adversarial Examples for Question Answering

## 背景・目的

QAタスクにおいて、モデルが解けないような問題を作って評価することが必要になってくる。
だが、これらを自動的に生成することは、問題の意味が変化したり、評価できなくなってしまう課題がある。

そこで、Human-in-the-Loopを用いて人間により、質問を作成するプラットフォームを作成した。

## 関連研究との違いは？

## 提案：解決に向けたキーアイデア

 実際にモデルが解答する上で文章中のどこに注目したのかを人間に見せ、それを下に質問を加筆、修正してもらう手法。

 !()[./img/wallance2019_ui.png]

## 結果:結局問題は解決されたのか．新しくわかったことは？

情報検索（IR）と深層学習モデル（RNN）を使って答えを提示し、質問を編集してもらった。

Adversarialが、編集してもらった場合の問題をつかてシステムの正解率を測定した。
横軸は、質問を全体のうちどれくらい見せたかを表している。

作成してもらった質問を使った方が正解率が低くなっていることがわかる。

!()[./img/wallance2019_round1.png]

!()[./img/wallance2019_round2.png]

## 感想

