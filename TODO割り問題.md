# 000 Hello World

ユーザーが自分の名前を入力します。コンピュータが、「Hello, <入力した名前>.」と出力します。

```mermaid
---
title: Hello World
---
flowchart TB
    id0((開始))
    id1[入力]
    id2[処理]
    id3[出力]
    id4((終了))
    id0 --> id1 --> id2 --> id3 --> id4
```

```mermaid
flowchart TB
    id0{分岐}
    id1[処理1]
    id2[処理2]
    id0 -- true --> id1
    id0 -- false --> id2
```


# 001 数字にする

ユーザーが入力した文字列を数字に変換して、その数字を表示する。ただし、ユーザーが入力した文字列が数字でない場合は、`"数字ではありません"`と表示する。

# 002 3の倍数

ユーザーに入力させた数字が3の倍数かどうかを判定する。 3の倍数の場合は`"3の倍数です"`、違う場合は`"3の倍数ではありません"`と表示する。

# 003 足し算

ユーザーに複数の数字を入力させて、すべての合計を表示する。ユーザーは数字をいくつでも入力できるようにして、"end"と入力したところですべての合計を表示すること。

# 004 計算機

ユーザーに加減乗除の記号(+-*/)と数字を入力させて、計算結果を表示する。ユーザーは記号と数字をいくつでも入力できるようにして、"end"と入力したところですべての計算結果を表示すること。
計算機を入出力と分離して1つのクラスとして実装すること。

# 005 ユーザーとの会話

ユーザーとの会話を開始する。最初にユーザーに名前を入力させ、次に入力された名前を使って、"こんにちは、◯◯さん"と表示する。その後、ユーザーに好きな食べ物を入力させ、"◯◯さんの好きな食べ物は△△ですね"と表示する。食べ物を複数入力できるようにすること。食べ物が2つ以上なら、「好きな食べ物は△△と、△△と、△△ですね」のように表示する。ひとつも入力しなかったら、好きな食べ物のことは表示しない。

# 006 名前のタテヨコ逆向き表示

ユーザーから名前を入力させる。その名前を、左から右、上から下、右から左、下から上にそれぞれ表示する。

```
例: 入力が「やっとむ」だったら、以下のように表示する。
やっとむ
や
っ
と
む
むとっや
む
と
っ
や
```

# 007 じゃんけん

ユーザーとじゃんけんをする。最初に、ユーザーに手を入力させる。その後、コンピューターの手と比べて、勝ち・負け・あいこのどれかを表示する。コンピューターの手はランダム(乱数)で決めること。

# 008 あっち向いてホイ

ユーザーとあっち向いてホイで勝負する。最初に、ユーザーに向きを入力させる。次に、コンピューターが自分の向きを決めて表示する。ユーザーとコンピューターの向きが一致したら、ユーザーの勝ち。一致しなかったら、ユーザーの負け。と表示する。コンピューターの向きはランダム(乱数)で決めること。

# 009 旗を立てる

コンピュータが「.」(ピリオド)を、横に10個、それを縦に10行表示する。ユーザーが列と行を数字で入力すると、その位置をの「.」を「P」に置き換えて、あらためて表示する。それを繰り返す。

```
こういう感じ:
..........
..........
..........
..........
..........
..........
..........
..........
..........
..........

1行目3列目を置き換えた状態:
..P.......
..........
..........
..........
..........
..........
..........
..........
..........
..........

何カ所かPに置き換えた状態:
..........
...P......
...P..P...
PPPPPPPPP.
...P..P..P
...P.....P
...P....P.
...P......
...P......
..........
```

# 010 交通費の精算

ユーザーが交通費を使った日付と金額を複数入力する。すべて入力したら、日付順に並んだレポートと合計金額を表示する。入力するとき、同じ日付であれば日付は省略できるようにする。

# 011 鬼滅隊士と呼吸

ユーザーが隊士の名前を入力すると、コンピュータがその隊士の呼吸を表示する。またユーザーが呼吸を入力したら、それを会得した隊士の名前を入力する。コンピュータが知らない隊士や呼吸が入力されたら、その場で適当な回答をでっちあげる。

# 012 ポケモンしりとり

ユーザーとコンピュータがポケモンの技しばりのしりとりをする。同じ技を使ったら負け。技はすべてひらがなとする。コンピュータは、答えられなくなったら「まいりました」と表示してしりとりを終了する。

# 013 ポケモンしりとり2

ユーザーとコンピュータがポケモンの名前しばりのしりとりをする。同じポケモンの名前を使ったら負け。このしりとりは特別に、最後の文字ではなく2文字目以降の文字が、次のポケモンの1文字目になればよい。例えば、`"ピカチュウ"`の次は`"チラーミィ"`、`"ミュウ"`の次は`"ウソッキー"`となる。コンピュータは、答えられなくなったら「まいりました」と表示してしりとりを終了する。

# 014 三目並べ

コンピューターとユーザーが三目並べをする。空いた場所は「.」(ピリオド)、ユーザーの手は「O」(オー)、コンピュータの手は「X」(エックス)で、3列かける3行で表示する。ユーザーが置く場所を入力し、コンピュータは空いた場所にランダムで自分の手を置く。
ここまでができたら、勝敗判定も自動でおこなうようにする。3つおなじ駒が並んだら、その人の勝利。並ばずに空いた場所がなくなったら引き分け。

# 015 ぼっち・ざ・ろっく歌詞検索

ユーザーが単語を入力すると、その単語を含む結束バンド(ぼっち・ざ・ろっく) の曲の歌詞を表示する。見つからなければ「ありません」と表示する。
歌詞が書いてあるテキストファイルをあらかじめ手で作っておき、それをプログラムから読み込むようにしてください。

# 016 ぼっち・ざ・ろっくの歌詞によく出てくる言葉

結束バンド(ぼっち・ざ・ろっく)の曲の歌詞の中で、よく使われている言葉を表示する。使われている回数も表示する。
歌詞から言葉を抽出するには、n-gramアルゴリズムを用いる。https://mojitoba.com/2019/09/23/what-is-ngram/ 


# 017 大阪へ行きたい

東京から大阪へは、新幹線なら2時間30分かかります。飛行機なら1時間30分です。車で行くと6時間です。高速バスだと8時間です。ただし、新幹線の運行時間は6時から21時です。飛行機は7時から19時です。高速バスは22時発車です。この情報を元に、現在時刻を入力すると一番早く着ける交通手段を出力するプログラムを書いてください。

# 018 ポケモン進化

ポケモンは種類によって進化のパターンが決まっています。それぞれの種類では一定のレベルに達すると別のポケモンに進化します。種類が異なれば進化するレベルも、進化結果のポケモンも異なります。このプログラムは、まず複数のポケモンの種類について、進化後の名前と進化レベルをユーザーに入力させます。入力が終わったら、今度はポケモンの種類とレベルをユーザーに入力させ、そのレベルでの進化後の名前を表示します。ユーザーが終了するまで、入力と表示を繰り返します。

# 019 ボケモノバトル

2人のボケモノがバトルするプログラムです(ポケモンではありません)。ボケモノはボケているので技は「つまむ」と「やすむ」しかありません。「つまむ」と相手のHPを1-10減らします(ランダム)。「やすむ」とHPが3増えます。HPが0になったら負けです。
ユーザーは自分のボケモノの名前を入力します。コンピュータはコンピュータ側のボケモノ名前をランダムに選びます。名前が決まったら、2人のボケモノのHPを10に設定します。ボケモノの名前とHPを表示します。ユーザーは自分のボケモノが使う技を指定し、その技を実行します。ユーザーの次にコンピュータが自分のボケモノが使う技を選んで実行します。どちらかのボケモノのHPが0になるまで繰り返します。勝負がついたら勝ち負けを表示します。HPが0になったボケモノの負けです。

# 020 逆ポーランド計算機

ユーザーが逆ポーランド記法の計算式を入力すると、その計算結果を表示する。式が間違っていたら、間違っている箇所を分かりやすく表示する。
逆ポーランド記法 https://qiita.com/Yuya-Shimizu/items/86a2246306bad769462d  

# 021 天気予報

ユーザーが都市名を入力すると、その都市の今日と明日の天気予報を表示する。都市名は日本語でも英語でも入力できる。都市名が間違っていたら、間違っている箇所を分かりやすく表示する。
天気予報はこちらのAPIを利用する https://weather.tsukumijima.net/

# 022 Spring Webの仕組み

ServletとSpring Webがブラウザからのリクエストを受け付けて処理する仕組みを、TomcatやSpringのソースコードとIDEのデバッグ実行を利用して調査し、仕様やフローチャートで表現してください。
