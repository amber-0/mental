# 課題　 --
全力のtodoアプリ(実用化)

## ①課題内容（どんな作品か）
- 全力のtodoアプリ

## ②工夫した点・こだわった点
- reactを使用（SPA対応、buildでindex.html生成）
- hostingを使ってfirebase上でデプロイ（firebase initでHostingを選択）
- Cloud Firestore上にデータ保管（テキストデータ、timestamp、boolean）
- PWAでスマホ対応(npx create-react-app 【アプリ名】 --template cra-template-pwa)
- googleログイン機能の実装（Auth）
- MaterialUIの使用（わかっていない）

## ③難しかった点・次回トライしたいこと(又は機能)
- 写経したがコードの内容が1割くらいしかわからない。
- PowerShell上でのエラーが非常に多かった。

## ④質問・疑問・感想、シェアしたいこと等なんでも
- PowerShell上でのエラーが多すぎたので、以下に色々記載しておく。
・node.jsのバージョン管理は、nodistを使わずにfnmを使う。
・管理者権限でPowerShellを開き、コマンドを実行すると何とかなることもあった。
・こいつでfirebase-toolsをインストール「npm install -g firebase-tools」
・MaterialUIはreact17.0.0までしか対応していない。
・バージョンの互換性は非常に重要。ここで大幅な時間ロスがあった。
・MaterialUIのコードはどこからどこまでが必要なのかよくわからない。
・ファイル「.env.local」にkeyを記載。冒頭に「.」を付けると隠しファイルになる。
・firebaseはver8で触っていた（npm i firebase@8.*）。
・reactはとにかく、コンポーネントを作ってインポートしまくる。
・一回デプロイした後のコードの修正はbiuldを挟む必要あり。
　npm run build→firebase deploy
・

- 今回参考にしたudemyの講座（4時間の動画を2倍速で見て、内容を写経したがトータル10時間以上かかった気がする…）
https://www.udemy.com/share/106rsg3@kcIfk_K47L9F4WKIavdo06khWy3P4ZhbfX2SXqXH8Zeb_lIA43cOjt7IJAPKsrD1Ww==/
- firebaseは壁にぶち当たりまくって、何をしているのかわからなくなったので、notionにまとめた（まとまってない）。
https://www.notion.so/firebase-bb60a804cab64a60b733a2fd521efba2
