# Portfolio

## About Me

笹倉 まお - Mao Sasakura  
email: maosasakura1998(gmail)

東京大学工学部機械工学科 2023年3月卒業予定

バックエンドエンジニアとしての就職を希望しています

github: [maosasa](https://github.com/maosasa)  
note: [maosasa](https://note.com/maosasa)  
qiita: [maosasa](https://qiita.com/maosasa)

* * *

## Works

### 落とし物共有SNS

道で見かける、交番に届けるほどでもない落とし物を位置情報と共に共有できるSNS。地図、リストの2種類の方法で閲覧できる。

code: [otoshimono](https://github.com/maosasa/otoshimono)  
page: [https://otoshimono-app.herokuapp.com/](https://otoshimono-app.herokuapp.com/)

<img src="https://github.com/maosasa/portfolio/blob/main/image/otoshimono.png?raw=true" width=500>

- 開発時期、期間：2021年　2週間（現在も改良中）
- 人数・役割：2人　基本機能の要件定義、実装
- 目的

    道でマフラーやハンカチが落ちていることがある。財布が落ちている場合は流石に警察に届けるが、貴重品でない場合は届けることはない。落ちたまま踏まれてしまうのは心苦しいが、良かれと思って道の脇にかけてしまうと、落とし主が見つけにくくなってしまう。高価なものでなくても、人によっては思い出が詰まったものもある。予期せぬ悲しい別れを減らしたい。

- 苦労した点

    マップを実装するにあたりはじめはgeodjangoを使用しようとしていたが、地理情報の扱い方の深い部分までの理解が必要であったため、短期間の開発には不向きだと考え、Google Map APIを使って簡略化した。
    
- 使用した技術
    - Python
    - Django
    - Bootstrap
    - Google Maps API

### スマートロック
    
ESPを使用しWiFiでスマートフォンから開閉できるようにしたスマートロック。筐体は3Dプリンタで製作した。

note: [スマートロックを作ったよ。](https://note.com/maosasa/n/nc453dd188249)

<img src="https://assets.st-note.com/production/uploads/images/59695392/picture_pc_3de935ba055c3608cde3d2f4f9bd0d78.jpeg" width=500>

- 開発時期、期間：2021年　2週間
- 人数・役割：個人開発
- 目的

    自宅の鍵をスマートロックに変えたかったが、市販のものは価格が高く、自作しようと考えた。

- 苦労した点

    見た目をスマートにしたかったので歯車3つを噛ませて動力を伝え、邪魔にならないところにモータを配置した。始めの設計ではサーボのトルクが強いため手動でサムターンを回せず、スマホの充電が切れた時に家に入れない仕様になっていたが、サムターンと歯車の間に90度の遊びを設けることで、自作スマートロックに不具合があっても鍵を開けられるようにした。

- 使用した技術
    - Arduino
    - 3DCAD

### 有向グラフを利用した、源氏物語登場人物の相関検索CLIツール
    
経路探索手法を用いて、「頭中将にとっての先帝は、頭中将 の 配偶者 である夕顔 の 配偶者 である光源氏 の 配偶者 である藤壺中宮 の 親」のように表示させるプログラム。任意の2人の登場人物の関係の全探索、最短経路探索、また直接の親子関係などが取れる。

code: [genji-graph](https://github.com/maosasa/genji-graph)

<img src="https://github.com/maosasa/genji-graph/blob/master/keizu.jpg?raw=true" width="500">

- 開発時期、期間：2018年　2週間
- 人数・役割：個人開発
- 目的

    Python入門の授業の最終課題として。授業でグラフのデータ構造について学んだので、それを活かせるものとして、複雑な家系図が特徴的な、源氏物語の家系図を扱うことにした。

- 苦労した点

    授業で習った一般的な有向グラフとは異なり、ある人iから別の人jへの関係性（親、子、婚姻関係）のタグ付をする必要があった。重みつきグラフの考え方を応用して、関係によって0,1,2の番号をエッジに付加することで、関係性のトラッキングを実装した。

- 使用した技術
    - Python

        構造体を利用してグラフのデータ構造を実装した

### 部活の仕事を効率化させるためのLINEbot『アイスちゃん』
    
毎度の練習の出欠確認や大会申込の締切確認など、今まで人力で行なっていた仕事を、GoogleAppsScriptを用いてカレンダーやスプレッドシートと連携して自動化させ、LINEグループに実装しました。簡単なif文によって、個人との会話もできるようにしました。

qiita: [GoogleAppsScriptで部活の仕事をbot化した](https://qiita.com/maosasa/items/aed6114be01ec78cbca8)

code: [club-line-bot](https://github.com/maosasa/club-line-bot)

<img src="https://github.com/maosasa/portfolio/blob/main/image/line_bot.png?raw=true" width="500">

- 開発時期、期間：2019年　1ヶ月間
- 人数・役割：個人開発
- 目的

    部活の幹部として行なっていた出欠確認などの仕事の無駄を省きたいと思ったため。元々はLINEの日程調整を用いて練習の出欠をとり、それを目で見ながら参加者一覧を打ち込み送信していた。

- 苦労した点

    部員が入力したスプレッドシートの値に表記揺れが多かったので、プログラム側で正規表現を用いて対応した。

- 使用した技術
    - Google Apps Script
    - LINE messenger API

### 80年分の太陽の黒点データを可視化するWebサイト

可視化するデータの期間を選択できるように、PythonとJavaScriptを用いてインタラクティブにデータの可視化を行うプログラムを実装した。扱いにくいデータの形だったが、うまく成形するようにプログラムして、80年分の毎日のデータを扱えるようにした。

code: [sun-data-web-page](https://github.com/maosasa/sun-data-web-page)

<img src="https://github.com/maosasa/portfolio/blob/main/image/sun_plot.png?raw=true" width="500">

- 開発時期、期間：2019年　2週間
- 人数・役割：個人開発
- 目的

    コンピュータシステムの授業の提出課題として。

- 苦労した点

    データの欠損が多かったところを、PythonによってCSVファイルを手直しして可視化できるような形に直した。

- 使用した技術
    - Python
    - Javascript
    - Flask

### Dreamee
    
社会人の先輩のキャリアパスキャリアパスをランダムに表示させ、新しい進路を発見することを狙いとしたAndroidアプリ

東大ガールズハッカソン2018 開催報告ページ: [http://www.todaishimbun.org/utokyo-girls-hackathon20181029/](http://www.todaishimbun.org/utokyo-girls-hackathon20181029/)

作品デモ動画:

[https://drive.google.com/file/d/1FkYIo38EF7CqEXEA4K7q4F9gC8RUHqIm/view?usp=sharing](https://drive.google.com/file/d/1FkYIo38EF7CqEXEA4K7q4F9gC8RUHqIm/view?usp=sharing)

プレゼン: [https://drive.google.com/file/d/1zZeKAiLf8vgBCeTC6CtyhfAIj48gI-Er/view?usp=sharing](https://drive.google.com/file/d/1zZeKAiLf8vgBCeTC6CtyhfAIj48gI-Er/view?usp=sharing)

<img src="https://github.com/maosasa/portfolio/blob/main/image/dreamee.png?raw=true" width="500">

- 開発時期、期間：2018年　2日
- 人数・役割：3人　UI作成
- 目的

    学生としてキャリアを考える上で、現在社会人として活躍する人々がどのような道を歩んできたのかが分からない、また、キャリアの選択肢がどれほどあるのかも学生にはわからないという問題を実感していた。ランダムに表示されるさまざまな社会人の経歴、ターニングポイントが手軽に見られるツールがあればロールモデルの発見に繋がるのではないかと考えた。

- 苦労した点

    スワイプ1動作でのキャリアパス情報の切り替えを提案し、ユーザーが心理的な負担を感じることなく、それまで興味の及ばなかった進路を発見できるように工夫した。

- 使用した技術
    - Java
    - Android

## Awards

- 東大ガールズハッカソン2018 最優秀賞

    制作したプロダクトは上記 [Dreamee](#dreamee)

## Programming Skills

- Python
    
    Googleの2ヶ月のインターンで使用したため、ライブラリの作成、ユニットテスト、依存関係への配慮などの基本的な実務が可能なレベル。
    
- C
    
    ポインタの概念は理解しており、リファレンスをみながらコードが書けるレベル。
    
- C++
    
    リファレンスを見ながらコードが書けるレベル。
    
- Google Apps Script
    
    普段Googleやその他サービスのAPIを利用するときに使っている。
    
    基本的な機能はリファレンスを見なくても書けるレベル。

- Go
    
    入門中。Goを習得すれば時代の最先端をいくエンジニアになれる気がしたので。tenntennさんのハンズオンに取り組んでいる途中。https://github.com/tenntenn/gohandson
    
* * *

## Other Skills

- TOEIC 850点　2021年2月
- TOEFL 83点　2020年6月
- 英検準1級　2016年2月
- HSK5級 153点　2020年9月
- フィギュアスケートバッジテスト2級　2019年7月

* * *

## Work Experiences
- matsuri technologies 2021年8月-
    - Profit Management部 インターン
    - ウェブマーケティング、PythonやGASによる業務の自動化を担当している。
- Google STEP Internship 2019年7月-2019年9月
    - ソフトウェアエンジニアとして翻訳チームに所属。
    - 自分1人でのプロジェクトを頂き、Pythonによる開発、評価、英語プレゼンを行った。
    - Google Style Guideに則ったコーディング、ユニットテスト、バージョン管理を学んだ。
    - 成果を評価していただき、Returning Internshipのオファーをいただきました。
- 家庭教師　2018年1月-
    - 中高生3名の指導経験があり、うち1名は現在も指導中。
    - 教科の勉強だけでなく、生徒の勉強に対する意識、スケジュール管理のサポートにも力を入れて指導している。
- 東進東大特進コース　チューター　2017年5月-2018年3月
    - 全国約100名の東大志望の生徒の担当として、電話による学習相談の業務を行った。
    - チューターが約30名の生徒に授業や添削を行う勉強会イベントでは、英語講師を務めた。

* * * 

## Other Experiences
1. 東大シャッフルランチ立上げ・運営  
[プロジェクト報告スライド](https://drive.google.com/file/d/1B9nIZhK3wJqKRvie8n6t4bw06ewpt4wx/view?usp=sharing)
1. 中高生向けのプログラミング授業・進路講演の企画運営  
[開催報告](http://swa.city-osaka.ed.jp/weblog/index.php?id=h543541&type=1&column_id=1263822&category_id=2216)
1. TeaTime TechLab運営  
[イベントレポート](https://drive.google.com/file/d/1fe4FZ0G_8gEGof8Knjy70bmdgqMjohAp/view?usp=sharing)
1. ものゼミTA  
[授業ページ](https://monozemi.akg.t.u-tokyo.ac.jp/)
1. 部活の仕事の効率化

