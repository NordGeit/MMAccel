# MMAccel

MMDにショートカットを追加するツール

## インストール

d3d9.dllとMMAccelフォルダをMikuMikuDance.exeと同じフォルダにコピーしてください。
MMAccelのd3d9.dllでMMEのd3d9.dllを上書きしてもMMEを使用できます。

インストールが成功すれば、MMDにMMAccelというメニューが現れます。

## 使い方

MMAccelメニューを開いて「キー設定」をクリックすると、キー設定のウィンドウが表示されます。

目的の動作を探して項目をダブルクリックすると入力待ち状態となります。
ここで割り当てたいショートカットキー押して、

* クリックで確定
* 右クリックでキャンセル

となります。

また、同時押しにも対応しています。

キーの解除は解除したい項目を右クリックでメニューを出して「解除」をクリックしてください。

## 設定

### タイマーの精度を上げる

FPS無制限時のフレームレートが上がったりします。
詳しく言えば`timeBeginPeriod(1)`を呼び出してタイマーの精度を上げます。

### クリックで入力状態を解除

数値などを入力しているときに別の場所をクリックすると入力状態が解除されるようになります。

## 以前のkey_map.txtについて

キー設定のウィンドウにkey_map.txtをドラッグアンドドロップすることで取り込むことができます。

## 注意事項

### MMDのバージョン

動作確認をMMD v9.32で行っています。それ以前のMMDでの動作は保証できません。

### MMEとの併用

MMAccelのd3d9.dllではMMEを動作させることが出来ますが、MMEのd3d9.dllではMMAccelを動作させることが出来ません。
また、MMEにおいてCtrl+Shift+Eが「エフェクト使用」で使われており、MMAccelで割り当てると割り当てた動作が行われるのと同時にMMEの「エフェクト使用」をクリックした状態になります。

## ソースコード

https://github.com/LNSEAB/mmaccel
  
## ライセンス

[MIT License](LICENSE)

(リポジトリのMikuMikuDance_v932x64は除く）

## 謝辞

MMEについてご教示くださいました舞力介入Pに御礼申し上げます。

-------------------------------------------------

Copyright (c) 2021 LNSEAB
