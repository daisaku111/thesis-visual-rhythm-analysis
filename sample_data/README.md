This directory includes a few sample datasets to get you started.

*   `california_housing_data*.csv` is California housing data from the 1990 US
    Census; more information is available at:
    https://docs.google.com/document/d/e/2PACX-1vRhYtsvc5eOR2FWNCwaBiKL6suIOrxJig8LcSBbmCbyYsayia_DvPOOBlXZ4CAlQ5nlDD8kTaIDRwrN/pub

*   `mnist_*.csv` is a small sample of the
    [MNIST database](https://en.wikipedia.org/wiki/MNIST_database), which is
    described at: http://yann.lecun.com/exdb/mnist/

*   `anscombe.json` contains a copy of
    [Anscombe's quartet](https://en.wikipedia.org/wiki/Anscombe%27s_quartet); it
    was originally described in

    Anscombe, F. J. (1973). 'Graphs in Statistical Analysis'. American
    Statistician. 27 (1): 17-21. JSTOR 2682899.

    and our copy was prepared by the
    [vega_datasets library](https://github.com/altair-viz/vega_datasets/blob/4f67bdaad10f45e3549984e17e1b3088c731503d/vega_datasets/_data/anscombe.json).
# Visual Rhythm Score Analysis for Thesis

卒業論文「都市空間における視覚的リズムと滞在行動の関係」の分析コードおよびデータセットです。
立川GREEN SPRINGS（実測）および調布駅前広場（シミュレーション）の空間分析を行いました。

## プロジェクト概要
Space Syntax理論を応用した独自指標「Visual Rhythm Score ($Q_i$)」を用いて、広場空間の快適性と滞在行動の関係を定量化しました。

## ファイル構成
* `analysis.py`: 分析および図表作成用のメインスクリプト
* `data/`:
    * `Type1.csv` - `Type4.csv`: 調布駅前広場のシミュレーションデータ
    * `tatikawa_data.csv`: 立川の実測データ
* `output/`: 生成されたグラフ画像 (Figures)

## 分析結果サマリ
* **Type IV（群島型）の優位性**: 
  * 視覚的ノイズ（高スコア域）を90%以上カット。
  * 快適領域（$Q_i < 1467$）の割合が 7.5% (現状) → 77.6% (提案) に向上。
* **統計的有意差**:
  * 現状と比較して効果量 $d=1.40$ (Large) での改善を確認。

## 環境
* Python 3.x
* pandas, matplotlib, numpy
