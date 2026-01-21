# Instacart 再購入予測

# 概要
Instacartの購買履歴データを用いて、
ユーザー×商品の再購入を予測する。

# データの事前処理
products.csv、order.csv、department.csvの欠損値やnullをis null を用いて確認した
orders.csvについては欠損値はなかったものの、days_since_prior_fielledカルムにおいて""の空欄がみられた。
→初回購入と考え、coalesceを用いて0に置換した。新たなカルムを作成する

