# ios_firebase_install

pod で firebase を追加する際のpodファイルの書き方について
詳細は以下記事を参照ください。

**iOSで共有Frameworkを利用した際に、podで追加したFirebaseが競合しクラッシュしてしまう問題の解決**
https://qiita.com/beckyJPN/items/bfe5829a0dd4f2adf506

## 注意事項
`GoogleService-Info.plist`
をプロジェクトに追加していないため、ビルドは通りません。

`myApps`
直下に、ご自身の `GoogleService-Info.plist` を追加することで
ビルドできるかと思います。

また、 `pod update` or `pod install` も必要です。
