# ラビットチャレンジ 深層学習day4  
  
##  Section1:強化学習  
  
要点    
・強化学習：行動選択の仕方を学習する機械学習モデル。  
・行動の結果として与えられる報酬を最大化するように  
行動原理を改善していく。  
・初期は、エージェントには環境についての知識が無い為、  
行動を通して探索する必要がある。一方で良い行動が  
見つかれば、それを利用した方がよい。  
・探索と利用はトレードオフになる。  
・方策勾配法などによって最適化する。  
  
##  Section2:AlphaGo  
  
要点  
・囲碁の世界チャンピオンに勝利したAlphaGoも強化学習を利用。  
・盤面やルールを数値化し、方策勾配法で学習する。  
・教師となる局面の評価には、モンテカルロ木探索を用いている。    
・AlphaGoを改良したAlphaZeroは自己対局のみから学習する。  
  
##  Section3:軽量化・高速化技術  
  
要点  
・深層学習の計算を高速化する為、分散深層学習等が用いられている。  
・データ並列化、モデル並列化、GPUによる高速化がある。  
・一方で、モデルの精度を維持しつつパラメータや演算回数を減らす  
工夫もされている。（モデルの軽量化）  
・量子化、蒸留、プルーニング等の手法が提案されている。  
  
##  Section4:応用モデル  
  
要点  
・MobileNets：モデルの軽量化・高速化・高精度化を実現するモデル。  
・Depthwise ConvolutionとPointwise Convolutionの組み合わせで軽量化を実現。  
・DenseNet：ResNetの様に、前の層から後ろの層へのパスを接続して学習させる。  
・InstanceNorm：各sampleの各チャンネルごとに正規化。  
  
##  Section5:Transformer    
  
要点  
・従来のニューラル機械翻訳は長さに弱い為、Attentionが誕生した。  
・研究の結果、RNNを使わずAttentionのみでも機能する事がわかった。  
・RNNよりはるかに少ない計算量でSOTAを実現。  
・Attentionを可視化すると、言語構造を捉えていることが多い。  
  
##  Section6:物体検知・セグメンテーション  
  
要点  
・物体検知：画像中の物体を位置も含めて検出する。（Bounding Boxを利用。）    
・セグメンテーション：各ピクセルに対し、単一のクラスラベルを与える。  
・MS COCO、OICOD、VOC、ILSVRCなどのデータセットが公開されている。  
・目的に合わせたデータセットを用いる事が重要。  
