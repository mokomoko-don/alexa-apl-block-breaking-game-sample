# ブロック崩しゲームサンプル(Block Breaking Game Sample)

「ブロック崩しゲームサンプル」は、APL 1.4で動作するブロック崩しゲームのサンプルです。

# ScreenShot

![スクリーンショット](https://raw.githubusercontent.com/mokomoko-don/alexa-apl-block-breaking-game-sample/master/images/block_breaking.png)

# DemoMovie
![DemoMovie](https://youtu.be/_vjMZPRAeG4)

# Features

このコードはAmazon Echo Showシリーズなどに実装されているalexa上で動作します。

APL1.4の新機能、「新しいジェスチャーのサポート」と「handleTick」を駆使し、ブロック崩しゲームを実現しました。

# Requirement

 * Alexaが動作する実機
 * AlexaDeveloperConsoleアカウント
 * 簡単なカスタムスキル作成の知識

# Installation

カスタムスキルとして動作させる方法のほかに、開発コンソールのAPLエディタ上で（APLソースコードのみで）動作させることもできます。

## 開発中スキルとして起動する方法

 * AlexaDeveloperConsoleにてHelloWorldスキルを作成(AlexaHostedSkill)
 * 任意のスキル名を入力
 * 「インターフェース」を押す
 * 「Alexa Presentation Language」を有効にする
 * 「インターフェースを保存」
 * 「対話モデル」→「JSONエディター」画面へ
 * /interactionModels/custom/ja-JP.json をコピーペースト
 * 「モデルを保存」して「モデルをビルド」する
 * コードエディタ画面へ
 * lambda配下のファイルをすべてコピーペースト
 * /lambda/APL/renderDocument_sample.json の524行目を実際の画像URLに差し替える（なくても背景無しで動作します）
 * 保存してデプロイ
 * 「テスト」画面へ
 * プルダウンの「非公開」を「開発中」に

## APLエディタ上で実行する方法

 * AlexaDeveloperConsoleにてHelloWorldスキルを作成(AlexaHostedSkill)
 * 適当にスキル名を入力
 * 「ビルド」画面にて、「マルチモーダル」画面へ
 * 「Visual」を押して「Create Visual Response」
 * 「コードをアップロード」
 * "aplEditor/apl_template_export.json"を読み込み
 * 画面右上の「テンプレートを保存」を押す

# Usage

## 開発中スキルとして起動する方法

実機から「アレクサ、＊＊＊を開いて」で起動
（PCのシミュレータでは未確認）

## APLエディタ上で実行する方法

APLエディタ画面にて、出力シミュレーションの下の実機出力ボタンを押す
（PCではプレビューモードでお試しください）

## 遊び方

タッチやドラッグでパッドを操作し、ボールを下に落とさないようにブロックを消しましょう。

パッドに当たるボールの位置によって、ボールの反射角度が変化します。

※ゲームクリア等の演出はありません。

# Note
2020年9月時点では動作確認済みです。今後の仕様変更等により正常に動作しなくなった場合、その動作は保証しませんのでご注意ください。
まれにブロックが消えないバグがあるようです。自信のある方は直してみてね！

# Author

* kyukkyu
* Twitter : https://twitter.com/Synoyan

# License

"ブロック崩しゲームサンプル(Block Breaking Game Sample)" is under [MIT license](https://en.wikipedia.org/wiki/MIT_License).

