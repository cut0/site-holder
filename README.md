## 概要
ブックマークするほどではないけど、後で読んでおきたいようなサイトを気軽に登録できるアプリケーションです。

## 利用方法
- グループ画面
  - サイトをまとめるグループを作成するページ
- サイト一覧画面
  - アイテムをクリックすることでサイトに飛べる。
  - アイテムを長押しすることでシェアできる。
  - textBoxにURLを入力することでサイトを登録できる。(一部取得できないサイトも有るため、今後修正する必要がある。)

## 使用した技術
- `Swift UI` :
  宣言的UIにより、開発効率を向上させるために採用
- `OpenGraph`(https://github.com/satoshi-takano/OpenGraph) :
  指定したURLからOGPを取得するために採用

## 反省点
- ユーザの登録したサイトをどのデバイスからもアクセスできるようにサーバーに保持しようと思ったが時間の都合上難しかった。
- 各ビジネスロジックに関してテストコードを書きたかったが技量と時間が足りなかった。
- UIをFigmaで設計してから開発したかった。

## 今後の展望
- ログイン機能とマルチデバイス対応の開発
  - `Firebase Authentication`と`Firebase FireStore`を検討中(金銭的なコストも開発的なコストも低いため)
- UIの改善