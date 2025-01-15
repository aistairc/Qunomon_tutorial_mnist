# 加工済みのMNISTデータセット

このリポジトリには、元のMNISTデータセットを加工したデータが含まれています。

## 作成者
 - **Author**: AIST AIRC

## 元のデータセットについて
- **元データセット名** :MNIST Dataset
- **作成者** :Yan LeCun, Corinna Cortes, Christopher J.C Burges
- **出典** :[MNIST公式ホームページ](https://yann.lecun.com/exdb/mnist/)
- **ライセンス** : Creative Commons Attribution-Share Alike 3.0 (CC BY-SA 3.0)

元データセットに関するライセンス詳細については、以下を参照してください:
[CC BY-SA 3.0 ライセンスの詳細](https://creativecommons.org/licenses/by-sa/3.0/)

---
## 加工後のデータセットについて
このリポジトリでは、元のMNISTデータセットに以下の加工を施しました:
1. 画像の正規化
    - ピクセル値の範囲を[0,255]から[-1,1]にスケール変換をしました。
2. チャネル次元の追加
    - データの形状を(60000,28,28)から(60000,1,28,28)に変更しました。
3. サンプルサイズの削減
    - 元データセット(60000枚の画像)から層化抽出法により、6000枚を選択しました。

加工内容を再現するためのコードは以下のファイルに記載されています:
 `notebooks/sandbox.ipynb`
 `notebooks/sandbox2.ipynb`

### ライセンス
加工後のデータセットも、 **CC BY-SA 3.0** ライセンスの下で提供されます。
このライセンスに基づき、以下を守ってください:
- 元データセットの作成者を明記してください。
- 加工後のデータを再配布する場合、同じライセンス条件（CC BY-SA 3.0）で提供してください。

---

## データのダウンロードリンク
加工後のデータセットは以下からダウンロード可能です。
- **ダウンロードリンク**:[Githubリポジトリリンク](https://github.com/aistairc/Qunomon_tutorial_mnist)

---
## 使用例
加工後のデータセットを利用したサンプルコードは `notebooks` ディレクトリ内にあります。

---

## 注意事項
商用利用を含む使用が可能ですが、本ライセンス条件を遵守する必要があります。
詳細については、以下のURLでライセンス全文を確認してください:
[CC BY-SA 3.0 ライセンス全文](https://creativecommons.org/licenses/by-sa/3.0/legalcode)