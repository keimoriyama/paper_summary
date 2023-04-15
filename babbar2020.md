---
id: "babbar2020"
aliases:
  - "babbar2020.md"
  - "On the Utility of Prediction Sets in Human-AI Teams"
tags:
  - "paper"
  - "Human-AI"
  - "CP"
---

# On the Utility of Prediction Sets in Human-AI Teams

## 背景・目的

複数の予測ラベルを出力する手法として、Conformal Predictionがある。
CPが出力するラベル数は大きくなる傾向があるという課題がある。
そのため、ラベル数が大きくなりそうなデータについては人間に予測を依頼し、そうではない場合モデルが予測するという手法を提案した。

## 関連研究との違いは？

[[vovk2005|vovk2005]]らが提案したConformal Predictionは近年興味をもたれつつある。
これ以外のCPベースの手法として、[[stutz2022]]や[[romano2020]],[[angelopoulos2020|angelopoulos2020]]がある。
マルチクラス分類を扱った手法として、[[mozannar2020]]や[[okati2021]],[[wilder2020]]がある。

これらの手法は全て、AIがどのデータについて予測するかを選択する手法になっているが、この研究では、人間に予測を依頼する際に、データだけではなく予測の候補も提示するような手法になっている。

## 提案：解決に向けたキーアイデア

[[angelopoulos2020]]の手法をベースにして提案している。
提案アルゴリズムは以下の通り。

!()[./img/babbar2020_method.png]

1~5行目は予測モデルを学習させ、6,7行目でDeferral Functionに用いる閾値を計算している。

## 結果:結局問題は解決されたのか．新しくわかったことは？

CIFAR-100からデータをサンプリングして実験を行った。
!()[./img/babbar2020_result.png]

上の表の右3列から、渡されるラベルの数は減っていることがわかる。
また、正解が含まれているものが多いことも確認できた。

## 感想

関連研究を読まないといけなさそうだと思う。
この論文の関連研究を読んでいく。

