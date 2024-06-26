# shinsui-rank-danmen
標高の代わりに浸水ランクで断面図を作成する（地理院地図ベース）

https://mghs15.github.io/shinsui-rank-danmen/

* [地理院地図](https://maps.gsi.go.jp/)の「断面図機能」を流用し、標高の代わりに浸水想定区域のデータを読み込ませ、「浸水深断面図」を作成する参照実装である。
* 標高タイルの代わりに利用したデータは、[重ねるハザードマップ](https://disaportal.gsi.go.jp/hazardmapportal/hazardmap/copyright/opendata.html)の洪水浸水想定区域（想定最大規模）等である。
  * ただし、地点ごとの詳細な値は格納されておらず、浸水深の幅（例：0.5～3.0m）のみが格納されているため、その幅の中での最大値を利用している（20.0m以上は、便宜的に30mと設定）。

> [!CAUTION]
> あくまで**参照実装**です。**このサイト自体を防災の目的で利用しないでください** 

![サンプル画像](sample-image.png "浸水クラスの断面図サンプル")

## 参考
* 地理院地図のソース https://github.com/gsi-cyberjapan/gsimaps
* ハザードマップポータルサイト https://disaportal.gsi.go.jp/hazardmapportal/hazardmap/copyright/opendata.html

