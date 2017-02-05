# preprocess の解説
## requirement
- pandas >=0.19.1
- numpy >=1.11.0

## What it is
<a href='https://resas.go.jp'>https://resas.go.jp</a>からダウンロードしたファイルを、

1. 欠損値を 全て numpy.nan に統一
2. 中業種コードごとに列を作成
3. 作成年を 2012 年に統一（人口関連は 2015 年のそれを利用）

し、市区町村コードで join した単一の csv ファイルを作成するスクリプト

## How to use
整形後のデータは<a href='../data' > ../data/ </a>に置いてあります。
各データの利用サンプルは <a href='../結婚出産に関する分析'>結婚出産に関する分析 フォルダ</a> をご参照ください。

<a href='resas_datamining_fromCSV.ipynb' > resas_datamining_fromCSV.ipynb </a> でデータ生成の再現が可能

1. Jupyter notebook ファイルなので、Jupyter notebookを起動し読み込み
2. あるいは写経

オリジナルのデータは preprocess 下に data フォルダを作成し、<a href='https://resas.go.jp'>https://resas.go.jp</a>からめぼしいものを直接ダウンロードし、それをzip解凍したフォルダを配置（ダウンロードリンクが発見しにくいので注意）