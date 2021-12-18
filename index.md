# Portfolio

## About Me

笹倉 まお - Mao Sasakura  
email: maosasakura1998(gmail)

東京大学工学部機械工学科 2023年3月卒業予定

バックエンドエンジニアとしての就職を希望しています

## Works

1. スマートロック
    
    ESPを使用しWiFiでスマートフォンから開閉できるようにしたスマートロック。筐体は3Dプリンタで製作した。
    
    note: [https://note.com/maosasa/n/nc453dd188249](https://note.com/maosasa/n/nc453dd188249)
    
   
    
    - 開発時期、期間：2021年　2週間
    - 人数・役割：個人開発
    - 目的
        
        自宅の鍵をスマートロックに変えたかったが、市販のものは価格が高く、自作しようと考えた。
        
    - 苦労した点
        
        見た目をスマートにしたかったので歯車3つを噛ませて動力を伝え、邪魔にならないところにモータを配置した。始めの設計ではサーボのトルクが強いため手動でサムターンを回せず、スマホの充電が切れた時に家に入れない仕様になっていたが、サムターンと歯車の間に90度の遊びを設けることで、自作スマートロックに不具合があっても鍵を開けられるようにした。
        
    - 使用した技術
        - Arduino
        - 3DCAD

2. 有向グラフを利用した、源氏物語登場人物の相関検索CLIツール
    
    経路探索手法を用いて、「頭中将にとっての先帝は、頭中将 の 配偶者 である夕顔 の 配偶者 である光源氏 の 配偶者 である藤壺中宮 の 親」のように表示させるプログラム。任意の2人の登場人物の関係の全探索、最短経路探索、また直接の親子関係などが取れる。
    
    code: https://github.com/maosasa/genji-graph
    

    - 開発時期、期間：2018年　2週間
    - 人数・役割：個人開発
    - 目的
        
        Python入門の授業の最終課題として。授業でグラフのデータ構造について学んだので、それを活かせるものとして、複雑な家系図が特徴的な、源氏物語の家系図を扱うことにした。
        
    - 苦労した点
        
        授業で習った一般的な有向グラフとは異なり、ある人iから別の人jへの関係性（親、子、婚姻関係）のタグ付をする必要があった。重みつきグラフの考え方を応用して、関係によって0,1,2の番号をエッジに付加することで、関係性のトラッキングを実装した。
        
    - 使用した技術
        - Python
            
            構造体を利用してグラフのデータ構造を実装した
            

3. 部活の仕事を効率化させるためのLINEbot『アイスちゃん』
    
    毎度の練習の出欠確認や大会申込の締切確認など、今まで人力で行なっていた仕事を、GoogleAppsScriptを用いてカレンダーやスプレッドシートと連携して自動化させ、LINEグループに実装しました。簡単なif文によって、個人との会話もできるようにしました。
    
    qiita: [https://qiita.com/maosasa/items/aed6114be01ec78cbca8](https://qiita.com/maosasa/items/aed6114be01ec78cbca8)
    
    code: https://github.com/maosasa/club-line-bot
    
 
    - 開発時期、期間：2019年　1ヶ月
    - 人数・役割：個人開発
    - 目的
        
        部活の幹部として行なっていた出欠確認などの仕事の無駄を省きたいと思ったため。
        
    - 苦労した点
    - 使用した技術
4. 80年分の太陽の黒点データを可視化するWebサイト
    
    可視化するデータの期間を選択できるように、PythonとJavaScriptを用いてインタラクティブにデータの可視化を行うプログラムを実装しました。扱いにくいデータの形でしたが、うまく成形するようにプログラムして、80年分の毎日のデータを扱えるようにしました。
    
    code: https://github.com/maosasa/sun-data-web-page
    

    
    - 開発時期、期間：2019年　2週間
    - 人数・役割：個人開発
    - 目的
        
        コンピュータシステムの授業の提出課題として。
        
    - 苦労した点
        
        データの欠損が多かったところを、PythonによってCSVファイルを手直しして可視化できるような形に直しました。
        
    - 使用した技術
        - Python
        - Javascript
        - Flask
5. Dreamee
    
    社会人の先輩のキャリアパスキャリアパスをランダムに表示させ、新しい進路を発見することを狙いとしたAndroidアプリ
    
    東大ガールズハッカソン2018 開催報告ページ: [http://www.todaishimbun.org/utokyo-girls-hackathon20181029/](http://www.todaishimbun.org/utokyo-girls-hackathon20181029/)
    
    作品デモ動画:
    
    [https://drive.google.com/file/d/1FkYIo38EF7CqEXEA4K7q4F9gC8RUHqIm/view?usp=sharing](https://drive.google.com/file/d/1FkYIo38EF7CqEXEA4K7q4F9gC8RUHqIm/view?usp=sharing)
    
    プレゼン: [https://drive.google.com/file/d/1zZeKAiLf8vgBCeTC6CtyhfAIj48gI-Er/view?usp=sharing](https://drive.google.com/file/d/1zZeKAiLf8vgBCeTC6CtyhfAIj48gI-Er/view?usp=sharing)
    
 
    
    - 開発時期、期間：2018年　2日
    - 人数・役割：3人　UI作成
    - 目的
    - 苦労した点
        
        スワイプ1動作でのキャリアパス情報の切り替えを提案し、ユーザーが心理的な負担を感じることなく、それまで興味の及ばなかった進路を発見できるように工夫しました。
        
    - 使用した技術
        - Java
        - Android


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
    

## Other Skills

- TOEIC 850点　2021年2月
- TOEFL 83点　2020年6月
- 英検準1級　2016年2月
- HSK5級 153点　2020年9月
- フィギュアスケートバッジテスト2級

## Experiences
1. 東大シャッフルランチ立上げ・運営
2. TeaTime TechLab運営
3. ものゼミTA
4. 部活の仕事の効率化

