
- #### `pulse programmer` (パルスプログラマー、別名：RAM)
  **説明**: 外部デバイスの一種。アプリケーションがロードされた際に、初期定義領域の(`par;`と`endpar;`で区切られた) 測定パラメータを読み込み、機器に設定する。また NMS ライブラリ関数によって、このパルスプログラマ RAM に NMS 固有パラメータや計算メソッドなどの取得、アクセスをプログラムできる
  ※この説明はドキュメントおよび参考（参照）サイトの内容を基に個人的な理解でまとめたものです。

  > NMS library functions allow the user to program the pulse
  programmer that controls acquisition and access NMS specific parameters, calculation
  methods and input/output procedures.
  ###### 和訳: NMS ライブラリ関数により、ユーザーは、NMS固有のパラメータ、計算メソッド、入出力プロシージャの 収集とアクセスを制御するパルスプログラマをプログラムすることができます。

  **TL;DR**: `par;`と`endpar;`で囲われた初期定義値をパルスプログラマに読み込ませ値を設定する

- #### `pulse sequences` (パルスシーケンス)
  **説明**: パルスシーケンスとは対象（の原子核）に対して、適当な時間間隔を空けて与える一つ以上のパルス波<sub>[^1]</sub>およびそのパルス（波）の配列、パルス列<sub>[^2]</sub>
  パルスをかけている間、対象（の原子核）の磁化は回転する。z軸方向を向いていた磁化がちょうどxy平面上に乗るまでに必要なパルスの長さを90度パルスという。
  ここでパルスをやめると、磁化は定常状態へ戻っていき振動が減衰していくように見える(縦緩和)。[^1]
  ※この説明はドキュメントの内容を基に個人的な理解でまとめたものです。
  [^1][1H通常測定_NMRの基本原理_パルスシーケンス(pulse sequence)](http://lab.agr.hokudai.ac.jp/ms-nmr/nmr/1h.htm#:~:text=%E3%83%91%E3%83%AB%E3%82%B9%E3%82%B7%E3%83%BC%E3%82%B1%E3%83%B3%E3%82%B9(pulse%20sequence))
  [^2][JEOL_パルスシーケンス](https://www.jeol.co.jp/words/nmr/9e0f9b375d4dbc3d7bb23cffeef1503434d1bded.html)
  
  **TL;DR**: 縦緩和や横緩和と言われる振動の減衰を観るために、パルスシーケンスというパルスの配列を設定する
