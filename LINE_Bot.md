# LINE Bot
とりあえず登録してみたのでなんか考える。

## サイトなど
登録はLINE Business Centerから
- https://business.line.me/

APIリファレンスなど
- https://developers.line.me/bot-api/overview

さっそくなんか作ってる人がいた、って案の定ますいさんかｗ
- http://qiita.com/masuidrive/items/1042d93740a7a72242a3




## メモ
- BOTはユーザからのメッセージをLINE Platformをプロキシにして自分で立てたサーバで受け取って、同様にメッセージを返す感じで動く
- アクセスはHTTPS
- メッセージボディ的なものはJSON

てことは、とりあえずHTTPSサーバを立てられないと話にならんのでは。

### HTTPSサーバ
ざっと調べても2008年とか2004年とかけっこう古い情報ばかり出てくるので、とりあえずGoogleさんで1年以内で検索してみて参考になりそうだったのがこのへんかな（まだ中みてない）

Let's Encrypt で手軽に HTTPS サーバを設定する
- http://qiita.com/ww24/items/9fa19594b4e3a8eb9b6f

光の速さのWEBサーバー(nginx)をlet's encryptでSSL化及びHTTP/2化。ついでにセキュリティ評価をA＋にする。
- http://qiita.com/sak_2/items/ff835b669c0a7e110b09

Let's EncryptとnginxでHTTP/2サーバを立てる
- http://inside.pixiv.net/entry/2015/12/10/153114

独自ドメインが使えないことを除けばHerokuで運用できそうな気がする
- http://blog.deraru.com/post/76779981593/herokuでsslを使う3つの方法
- http://qiita.com/yuya_takeyama/items/0660a59d13e2cd0b2516#_reference-edae6ffa45aab9afe857

### つわけでHeroku

Heroku導入メモ
- https://gist.github.com/konitter/5370904

Node.jsのExpressで作ったサーバーをHerokuで動かす
- http://qiita.com/awakia/items/26eae40afb1c9ad76161

Express 4 をはじめよう
- http://qiita.com/hoshi-takanori/items/2128a6cf1dbb533379a2

