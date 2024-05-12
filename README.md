# shinsui-rank-danmen
標高の代わりに浸水ランクで断面図を作成する（地理院地図ベース）

* [地理院地図](https://maps.gsi.go.jp/)の「断面図機能」を流用し、標高の代わりに浸水想定区域のデータを読み込ませ、「浸水深断面図」を作成する参照実装である。
* 標高タイルの代わりに利用したデータは、[重ねるハザードマップ](https://disaportal.gsi.go.jp/hazardmapportal/hazardmap/copyright/opendata.html)の洪水浸水想定区域（想定最大規模）等である。
* ただし、地点ごとの詳細な値は格納されておらず、浸水深の幅（例：0.5～3.0m）のみが格納されているため、その幅の中での最大値を利用している（20.0m以上は、便宜的に30mと設定）。

![サンプル画像](https://raw.githubusercontent.com/mghs15/shinsui-rank-danmen/main/sample-image.png?token=GHSAT0AAAAAAB4W7LSC54TD7357OHNWYI2KZSATJOQ "浸水クラスの断面図サンプル")

## 参考
* 地理院地図のソース https://github.com/gsi-cyberjapan/gsimaps
* ハザードマップポータルサイト https://disaportal.gsi.go.jp/hazardmapportal/hazardmap/copyright/opendata.html

