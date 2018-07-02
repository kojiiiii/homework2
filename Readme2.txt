課題１
ガンマ変換を用いてトーンカーブのコントラスト変換を行った。
コントラスト変換の度合いを０～100に設定した。
途中の文でframeへの代入式で分母に0が来てしまう場合があったので、
場合分けをして0ではなく、近似して0.01を代入するようにした。
参考にしたURLは
https://algorithm.joho.info/programming/python/opencv-gamma-correction-py/
で、ソースコードの部分のガンマ変換を参考にさせてもらった。


課題２
今回は普段のRGB空間をHSV空間に変換できるようにした。
cvtColorの引数にCOLOR_RGB2HSVを与えた。
参考にしたURLは
https://bi.biopapyrus.jp/ia/opencv/color-space.html
で、中間のほうにあるHSV空間の項目のソースコードを参考にさせてもらった。

課題３
一次微分フィルタを用いてフィルタリングを行った。
一次微分フィルタは、画像から輪郭を抽出する空間フィルタ。
一次微分を計算することで、注目画素の左右・上下の画素値の変化の傾きが求まる。
画像の輪郭は画素値の変化が大きいため、微分した画素値が大きい箇所が輪郭となる。
参考にしたURLは
https://algorithm.joho.info/programming/python/opencv-differential-filter-py/
で、中間より少し上らへんにある方法②というソースコードを参考にさせてもらった。



