# 医用画像識別
MRI画像の腫瘍の有無による識別をしてみましょう．

## データ
Datasetディレクトリにデータが入っています．  
> Dataset/  
> 　├ train.tar.gz  
> 　　　├ 0/  
> 　　　　　├ 1.png  
> 　　　　　├  :  
> 　　　　　└   
> 　　　└ 1/  
> 　├ val.tar.gz  
> 　└ test.tar.gz  
0が腫瘍無し，1が腫瘍あり画像です．  

## 方法 
* trainディレクトリに入っているデータを学習データとして，testディレクトリに入っているデータの認識をしましょう
* valディレクトリに入っているデータは検証データとして用い，epoch数やハイパーパラメータの調整に使ってください
* 識別器は何を使ってもOKですし，複数試してみるとなお良いです
* 特に今後のためにCNNは試してみましょう
* ちなみに[VGG-16](https://arxiv.org/abs/1409.1556)を用いて85~90%位の認識率です

## 提出方法 
* 以下の内容ををtexでまとめてpdfで提出してください
	* 必須：用いた手法の内容と認識率，混同行列
	* 推奨：正解・不正解した画像の傾向解析
* 抵抗が無ければ，ソースコードをgithubにアップロードしてそのリンクを教えてください


