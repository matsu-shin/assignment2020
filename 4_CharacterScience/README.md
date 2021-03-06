# 文字画像解析（フォントの印象分類）
フォント画像とその印象語が関連付けられたデータセットを用いて，特定の印象語に対し，フォント画像のOne-vs-Restの2クラス分類を行いましょう．

## データセットの準備
1. 以下のリンクから本ディレクトリにデータセットをダウンロード<br>https://www.cs.rochester.edu/u/tchen45/font/font.html
2. Dockerfileに従って環境構築
3. preprocess_data.pyを実行
-> dataset/fontimage_preprocessed/に前処理を施したフォント画像データが，fontName_tagWord.csvにフォントと印象後の関連付けリストがそれぞれ保存される．

## データセットに関する注意事項
上記のリンクからダウンロードしたデータセットでは，taglabelフォルダにblank fileがあるため，taglabel.zipを解凍したものと置き換える

## 内容
* データを任意の割合（7:3など）で学習データとテストデータに分割
* ある印象語を指定し（"formal"など），それに関連付けられているか否かを2値ラベルとしてフォント画像を識別するように識別器を学習
* テストデータを識別し，認識率とどのような画像が正しく（あるいは間違って）分類される傾向にあるか確認する

## 提出方法
結果をLaTeXでまとめ，pdfで提出してください．  
抵抗が無ければ，ソースコードをgithubにアップロードしてそのリンクを教えてください．

## 参考
本課題はやや難易度が高いため，昨年度卒業生が作成したコードを添付しています（reference.zip）．難しければそれを参考に実装してみてください．


