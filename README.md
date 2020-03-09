## 🚀 HiraganaTranslationApp
- 漢字をひらがなに変換するアプリです。

<img width="340" alt="スクリーンショット 2020-03-09 0 34 42" src="https://user-images.githubusercontent.com/38596913/76198230-0846d200-6231-11ea-90c8-df0b959cdee5.png">


## 📖 ライブラリ管理
- Carthage version: 0.34.0 

## 🧘‍♀️使用ライブラリ
### ネットワーク通信
- [APIKit](https://github.com/ishkawa/APIKit)

## 👮 静的管理ツール
- [SwiftLint](https://github.com/realm/SwiftLint)

## 🐱 GitFlow
- master
  - プロダクトとしてリリースするためのブランチ。リリースしたらタグ付けする。

- develop
  - 開発ブランチ。コードが安定し、リリース準備ができたら master へマージする。リリース前はこのブランチが最新バージョンとなる。

- feature branches
  - 機能の追加。 develop から分岐し、 develop にマージする。

![TBHkD](https://user-images.githubusercontent.com/38596913/75508280-eaa28d00-5a26-11ea-9d78-04a7a143ff06.png)

## 🧑‍💻 設計
- MVC

![01-MVC-Diagram-480x241](https://user-images.githubusercontent.com/38596913/75508274-e5ddd900-5a26-11ea-9228-23578f45b09c.png)

## 🌈 ViewControllers
- TranslationViewController
  - 画面上部の入力エリアにワード(漢字)を入力し、結果を出力エリア:UITextViewに表示する
  
## 🌍 API
- ドキュメント

[ひらがな化API ｜ソフト・アプリ開発のAPIなら【gooラボ】](https://labs.goo.ne.jp/api/jp/hiragana-translation/)
``` 
$ curl -H "Content-type: application/json" -X POST -d '{"app_id":"[appId]", "sentence":"漢字が混ざっている文章", "output_type":"hiragana"}' 'https://labs.goo.ne.jp/api/hiragana'
```

## 🏋️ 導入方法
```
carthage update --platform iOS
```

## 🎡 必要条件
- Xcode 10.2 or later
- iOS 12.0 or later
- Swift 5.0 or later

## ⚠️ 注意事項
- [API利用登録 ｜ソフト・アプリ開発のAPIなら【gooラボ】](https://labs.goo.ne.jp/jp/apiregister/)

## 🎉 クレジット

![sgoo](https://user-images.githubusercontent.com/38596913/76199018-6aec9d80-6232-11ea-978d-3a73b8d7f332.png)

