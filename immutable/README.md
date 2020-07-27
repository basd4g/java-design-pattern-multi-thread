# Immutable パターン

壊したくとも、壊せない

Java言語で学ぶデザインパターン入門 マルチスレッド編
第2章 pp85-112

## 実行

```sh
$ ls
Main.java
Person.java
PrintPersonThread.java
README.md
$ javac *.java
$ java Main
# ctrl+Cで中断
```

## Immutable パターンとは

Immutable ... 不変の, 変わることがない

フィールドの値が変わることがないクラスであれば、インスタンスの状態が変わらないことが保証されているので、複数スレッドから同時にアクセスするときに排他制御の必要がないので、パフォーマンスが向上する

インスタンスの状態が変わらないことが保証されている
-> 排他制御の必要がない
-> パフォーマンス向上

対義語 ... mutable (変わりやすい)

クラス設計には不変性 (immutability) を意識するべき

## Immutable なクラスの特徴

### フィールドの値を変更するメソッドがない

- setName, setAddress などの値を変更するメソッドがない

### クラスをfinalで宣言している (必須ではない)

- サブクラスを作れない
- フィールドの値を変更するメソッドを追加できない

### フィールドをprivateで宣言している (必須ではない)

- クラス外からフィールドの値を変更できない

### フィールドをfinalで宣言している (必須ではない)

- フィールドに値が再代入されることがない
- 誤って再代入したらコンパイルエラーになる

## いつ使うべきか

- インスタンス生成後, 状態が変化しないとき
- インスタンスが共有され, 頻繁にアクセスされるとき
- mutable と immutable の対を作れるとき

## 不変性を守るために

- プログラムのコメントや API ドキュメントで 不変性について明記しておく
- フィールドが保持しているインスタンスをそのままgetterメソッドの戻り値にしない
- コンストラクタに引数として渡されたインスタンスをそのままフィールドに代入しない

## Immutable な標準クラスライブラリのクラス

- java.lang.String
- java.math.BigInteger
- java.util.regex.Pattern
- java.awt.Color
- java.lang.Void
- java.lang.Short (以下, 基本型のラッパークラス)
- java.lang.Ingeter
- java.lang.Long
- java.lang.Float
- java.lang.Double
- java.lang.Character
- java.lang.Byte
- java.lang.Boolean

