# コーディングファイル
EJS / Sass / JS 使用時のgulp環境

##　導入方法
ターミナルで 'npm i' を入力
node moduleがインストールされたら 'npx gulp'で起動

## 納品時
'npx clean'で生成されているpublicフォルダが削除されるので、
削除後にもう一度'npx gulp'でファイルを生成してからpublicフォルダ内のものを納品

## ejs使用について
ページが増える場合はejs-config.jsonにページ情報を追加
追加内容はaboutを参考に
ejsフォルダ内にページのフォルダを作成し、その配下にindex.ejsと_main.ejsの2つを作成すればコンパイルしたときに
aboutフォルダの中にindex.htmlが作成されます。

##　Sassについて
FLOCSSを採用
基本的にはobjectフォルダ内、projectに追加していき、
共通部分などはobjectのcomponentに追加
※visually-hiddenファイルは画面には表示させないけど、スクリーンリーダーに読ませるような要素に使用
