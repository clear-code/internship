# 7月の振り返り

## 期間
7/1 から 7/23

## やったこと
- 6月の振り返りをまとめ、7月の目標をたてた
    - 目標: droonga を使ったサンプルアプリケーションの作成

- groonga-client 関連の作業
    - table_create, column_create, load をサポート
    - 0.0.2 リリース
- groonga-command 関連の作業
    - predicate メソッドを TableCreate, ColumnCreate に追加
    - 1.0.3 リリース
- gqtp (1.0.4) のリリース
- 以上のリリースに関連して、アップデートドキュメントを書いた

- groonga を使った epub-searcher が完成
- epub-searcher について、groonga-client を使ってファイル登録ができる
  ようにした

- fluent-plugin-droonga 関連の作業
    - handler
        - table_create, column_create, add コマンド追加
    - adapter
        - select コマンド追加
    - express-droonga と fluent-plugin-droonga を繋げる

- 森さんから droonga の今後の実装についての説明を受けた
- fluent-plugin-droonga add の API についての相談

## できなかったこと
- droonga と epub-searcher をつなげて、「droonga のサンプルアプリケー
  ションの作成」とする所までは行かなかった
- fluent-plugin-droonga の README を編集していたが、ドロップした

## 思ったこと
- どこに対して何をテストするのが良いのかよく理解できていなかった
- 自分が次にやるのは何か、小さい粒度で考えられていなかった
- コミットメッセージの記述はまだそれなりに重い作業で、メッセージを書く
  前にやっていたことを忘れそうになるが、単純に慣れの問題だと考えており、
  経験を重ねてコミットメッセージをうまくパターン化できれば良いと思う

## できるようになったこと
- どこに対して何をテストするのかについて
    - おおまかな基準を理解することができた
        - 階層で考える
        - 依存を小さくする
