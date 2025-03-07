# 外耳道圧力変化を用いた無発声発話認識手法の提案

## 背景：
音声操作の課題として、「環境ノイズに大きく影響される」「静かな空間で使用しにくい」「個人情報の漏洩につながる」といった点が挙げられる。

## 目的：
外耳道の圧力変化を用いることで無発生発話を取得し、パスワードなどを秘匿入力できるような新たなインタフェースを提案する。

## 現時点での成果：
### OpenEarableの使用
OpenEarableを用いることで、無発声発話時の外耳道圧力変化を取得することができた。

### 母音と単語に分けて無発声発話を取得
母音はAIUEOを取得。単語は「Ongaku」「Saisei」「Teisi」「Tugihe」「Modoru」を取得。

### SVMの試行
1発話当たりの
・平均
・標準偏差
・最大
・最小
・1発話あたりの最大から10データの平均
・1発話あたりの最小から10データの平均
・DTW距離
を説明変数として試行

## これからの目標
### CNNの実装
