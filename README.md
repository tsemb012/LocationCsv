# LocationCsv

prefecture_csv
　・都道府県・県庁所在地の情報
　・エクセルで自作
　・都道府県情報はほとんど更新されないはずなので放置する予定
　・https://uub.jp/pdr/s/cap_4.htmlから引用

city_name_csv
　・市区町村の名前情報
　・読み方・ローマ字の表記などの情報が入っている。
　・名前は"city_name"に統一する。(クライアントも同様)
　・スクレイピングできないので、下記サイトから手動で取得するように
　・半年に一度くらい更新する。/ 廃止になった市区町村は表示されないので、ここにデータがなかった場合クライアント側でエラー表示をするように
　・https://postaladdress.jp/municipality/download

city_latlng_csv
　・市区町村の緯度経度情報
　・名前は"city_latlng"に統一する。(クライアントも同様)
　・csv_name_csvと統合するように、city_idが合致しない場合はスキップするように(Androidの実装と合わせるように)
　・https://github.com/code4fukui/localgovjp/
