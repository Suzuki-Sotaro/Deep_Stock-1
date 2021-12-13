# FXAI 
こんにちは、AIエンジニアの鈴木です。
この度着想から4年かけて「自動で稼ぐAI」を開発いたしました。

## 「自動で稼ぐAI」とは？
このプログラムは端的に表すとAIを搭載した自動売買プログラムです。<br>
では普通のアルゴリズム取引とは何が違うかというと、一般的なアルゴリズム取引は決まったルール（例えば最も簡単なルールだとゴールデンクロスとデッドクロス）に従って売買取引を行いますが、このプログラムは「自動で情報を収集し、自動で学習し、自動で売買するプログラム」だということです。<br>
具体的には<br>

①まずクラウド上で毎週末に自動で過去の株価、為替レート、先物、経済指標、その他SNSの情報を収集しデータとして蓄積します。<br>
②次に、そのデータをクラウドで自動でAIに学習させます。ここでの重要なポイントは決められたパターンで学習をするのではなく、アンサンブル学習、つまり様々なモデルを試し、どの情報がその時代に最も影響するかを数値化し、最適なモデルを選べるという点です。モデルは主にSVD、MLP、RNN、LSTM、GRUから選び、その中でパラメータの調整を行います。<br>
③最適なモデルが選ばれたら、平日の取引時間帯にリアルタイムで売買判断を予測し、クラウドからクライアントへ判断結果を送ります。<br>
④各証券会社の自動売買プラットフォームで、送られてきた売買判断をもとに自動売買をします。<br>
このように、毎週AIを時代に沿って最適化できるので、何も手を加えずとも半永久的に成長し続けることのできるプログラムとなっています。<br>
ちなみに個人的には「自動で稼ぐAI」という呼び名は好きでは無いのですが、万人に刺さる言葉として、あえてこのような呼び名にしました。

## プログラムの導入方法
このAIは為替証拠金取引(FX)のEUR/USDで最もパフォーマンスが良かったので、自動売買ができるのはEUR/USDのみとなります。その他通貨、株、債権、コモディティ、暗号資産はもテスト中ですので、良いパフォーマンスが出れば追加でアップロードしていきます。<br>
そして現在、このレポジリトリにはEX4ファイルが一つアップロードされています。なので、売買ができるプラットフォームはMetaTrader上のみとなります(推奨はOandaJapan)。近々、どの証券会社のプラットフォームでも対応できるようなソフトウェアの開発を計画中です。<br>
では具体的な導入方法です。<br>
①まずこのレポジリトリ内の「FXAI.ex4」ファイルをダウンロードします。<br>
②次に証券会社のMetaTraderを立ち上げ、「FXAI.ex4」ファイルを「Experts」ディレクトリに加えます。<br>
③外部変数として名前と生年月日を入力する欄がありますので、TaroYamadaのようにアルフファベットのフルネームを挿入してください。生年月日は20010101のように空白を開けずに入力してください。名前と生年月日をクラウド上で照合し、売買判断をMQL4ファイルに送り、MT4上で売買することができます。<br>




## 開発経緯
僕は5年前、ある一つの記事に出会いました。それは野村総研とオックスフォード大学が発表した「2030年までに2015年比で約50%の労働人口がAIとロボットに置き換わる」という衝撃的な記事でした。<br>
これは分かりやすく例えると、自分達の友達や親戚などで働いてる人たちの半分は2030年にクビになるということです。つまり新しい時代の仕事を模索しなければAIやロボットに今の職を奪われることになります。
それほどAI、そしてAIが巻き起こす第4次産業革命というのは社会を変えていくのだと気付いた時、僕はAIを誰よりも深く学び、AIを使ってで世の役に立ちたいと思うようになりました。<br>

## 最終的な目標
僕には一つの理想があります。それは全ての産業の生産過程において、上流、中流、下流を全て人工知能によって生産、制御し、そのエネルギー源を再生可能エネルギーによって賄うことができるなら、
人類は誰も働くことなく、「衣」「食」「住」を安定的に手に入れることができるのではないか、という仮説をもとに社会にAIを浸透させていくことです。<br>
以前イーロンマスクが人型ロボットを2023年に生産開始すると発表した際、彼は人型ロボットと同時にベーシックインカムも実現しなくてはならないと発言しています。つまり生産性を大幅に高めれば誰もが一定の所得を得ることは可能なのです。





