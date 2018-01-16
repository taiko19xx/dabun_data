BTC/JPYを売買するボットを組み立ててたんですが、何か一気に下がって大混乱なので一旦中止...。

どんなのかというと、[bitFlyerのAPI](https://lightning.bitflyer.jp/docs?lang=ja)が[PubNub](https://www.pubnub.com/)を使ったリアルタイム情報を配信しているので、それを使って売ったり買ったりする感じでした。  
まだ実運用ではなくて、シミュレーションレベルだったのが幸い？

他には、グラフ可視化にElasticsearch+Kibana、結果の通知にSlackを使っていました。

Elasticsearchは初めて使いましたが楽で良いですね。Kibanaで簡単に可視化できるのも高ポイントです。
Javaなので大分重くなるのがネックですが、そこさえフォローできれば色々詰め込めそうです。[Elasticsearch Service](https://aws.amazon.com/jp/elasticsearch-service/)はt2.microだと頼りないから、t2.mediumくらいは欲しいかな...。

Slackは特に説明いらず。Endpointにメッセージ投げるだけなので簡単。  
一人チームを運用しているのでそこに突っ込んでました。

まぁ、BTCでせこせこ稼ぐよりもJPYちゃんと稼げるようになれって事ですね。  
働くって素敵。いも。
