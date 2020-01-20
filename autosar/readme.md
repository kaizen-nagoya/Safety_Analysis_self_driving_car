自動車用のOS、通信規約、道具類などを規定しているAutosarは、ISO OSEKとISO/IEC POSIXの自動車産業における設計例である。

WTO/TBT協定によれば、国際的な調達は、ISO, IEC, ITUなどの国際規格を仕様記述の出発点として参照することを推奨している。

Autosarも、ISO OSEK及びISO/IEC POSIXを参照している。自動車分野はISOのTC22で審議しておりISOの単独文書。POSIXはIT分野でISO/IEC JTC1 SC22で審議しておりISOとIECの合同文書。

IEEEはEthernet, Wi-Fiなどを規格化し、ISO, IECと協力して関連規格を出版している。ISO, IEC, IEEEの共同文書も相当数ある。

SAEはアメリカの自動車技術会相当の組織。misraはイギリスにある自動車ソフトウェア団体。

それぞれの名称の出現頻度は下記。

|standard|count|organization|
|:--|--:|:--|
|osek| 176|ISO TC22|
|POSIX| 96 |ISO/IEC JTC1 SC22|
|ISO|2297||
|IEC| 138||
|IEEE|300||
| sae | 723|Society of Automotive Engineers|
| misra| 410||

#背景

Toppersプロジェクトで ISO Osekに対応したオープンソースを発行する事業に参加し、標準化、安全分析、MISRA C適合、訓練などに参加してきた。また、TOPPERSプロジェクトのAutosar環境であるATKを実機なしで模擬試験できるソフトウェアを追っかけている。

TOPPERS/ATK2カーネル向け実機レス環境(athrill2)
https://qiita.com/kanetugu2018/items/75dadc340f3db2a344ab

OS及びC言語及びTCP/IP通信ソフトウェアのC言語規格およびPOSIXへの適合試験を行ってきた。

Posix Test Suite docker downloads, tar, install
https://qiita.com/kaizen_nagoya/items/f1e24be04a2405ede00f

Osekに基づいたAutosarへの対応においてもいくつかの視点で評価を行ってきた。
当初は、現在のclassic版だけであったが、Adaptive版についてもPOSIX対応の延長で対応してきた。

初めて検討する分野では、まず参考文献の参考文献を洗い出し、入手可能性を検討する。
参考文献の入手は時間がかかったり、お金がかかたりすることがある。そのため、最初に着手しておかないと、費用の見積もりを過小評価してしまうかもしれないからである。

参考文献の参考文献の入手性を確認したら、入手できた範囲の文献の用語頻度一覧と、略語集を作る。

今回、用語頻度一覧から着手しているのは、これまでに一度は入手可能性を確認した文書であることと、ISO/IEC JTC1 SC7から、ISO TC22への国際的なliaison(情報交換担当)として両委員会の公式文書をReviewしてきた過程において、各文書のNormative Referenceの入手可能性を検討してきた経緯があるからである。


# 文書入手

Autosar単語帳(作業中)
https://qiita.com/kaizen_nagoya/items/0927727a94b157df2df8

目次から一つづつファイルを入手しようとすると、最新ではない文書にぶつかったり、文書が一覧に見当たらないという現象に出会った。

そこで、上記URLの最後に記載した、一覧で一括入手できる方法によった。

# PDFのText変換

辞書作成のために、PDFをText変換した。

プログラミングの用語一覧の場合には、数字や_などの記号で、変数名、関数名、定数名で使うことができる文字を含んだ、なるべく長い文字列で一覧を作成する。

標準文書では、数字や_, -, などの記号を省略し、単語として同じ意味で使っている言葉はなるべく頻度を集計できるような方向での処理を行う。ただし、複数形、過去形などの変化系はあえて統合せず、文字列として現れるままで集計している。

これは、過去の難度かの複数形、過去形などの統合の処理では、別の意味で使っている用語を、文字列の並びがたまたま同じになるために同一の語として集計してしまったり、結果として分析のための精度が作業量に比較して向上しないという経験則による。

作業はdocker上で行った。どこからでも作業を再開できるようにdocker hubに保存している。

# 用語頻度



Autosar 単語検索　略号等
https://qiita.com/kaizen_nagoya/items/f8cb1295104b7d58363d


英語(38) 　複合語と複数の単語の一分類　https://qiita.com/kaizen_nagoya/items/219fd0bde3731f0881ed

作業記録 Autosar単語帳の分割の抜け漏れ
https://qiita.com/kaizen_nagoya/items/15b4011a68ce0ba81e6e


# 略号一覧

略号のfull spellingの確認のため、全文書の略号一覧を統合中である。
参考文献一覧の作成と一緒に作業中。


Autosar文書、参考文献、略号一覧（作成中）
https://qiita.com/kaizen_nagoya/items/2325b0156bc7fcf5a96d

普段はこの作業から始めるが、今回は逆順である。
これまで、複合語と複数の単語に分類することは、あまり意識してこなかった。
今回は、プログラミングですぐに用いることを想定するのではなく、プログラミングの変数名などを含むため、複合語を分解し、技術的な概念分布を検討することを目的とすることにした。

英語(2) まぎらわしい、間違えやすい、行き違いの多い略号worst 10(候補24)
https://qiita.com/kaizen_nagoya/items/0bff5dbb72208053489b

英語(3) 仮説・検証(88)用語の衝突(用語・用例募集中)
https://qiita.com/kaizen_nagoya/items/6a8eb7ffaa45eeb16624


#道具類

作業経過で利用している道具類は次の通りである。それぞれの作業で出たエラー類は別記事として整理している。


## docker
今日のdocker error : Error response from daemon: error while creating mount source path
https://qiita.com/kaizen_nagoya/items/1ff3550c4ef1c545ce12

## ubuntu

## bash

今日のbashエラー：No such file or directory(解決)
https://qiita.com/kaizen_nagoya/items/4bcf2ebdce3b475a808a

shell の種類と版
https://qiita.com/kaizen_nagoya/items/ab715ffeceb8617f11ca

## pdftotext 

PDFファイルの文字誤変換
https://qiita.com/kaizen_nagoya/items/49ce6e8cead58c646534

## sed

今日のsed error:unknown option to `s'
https://qiita.com/kaizen_nagoya/items/8e8c4efdb6869f965b54

## awk

## 表計算ソフト

## grep

grep　操作間違いなどhttps://qiita.com/kaizen_nagoya/items/2f14e895175908c296ca

## macOSテキストエディタ, mi.app

四角い領域の切り取り、切り貼り
https://qiita.com/kaizen_nagoya/items/ba3661d4e224acdf1b04

#参考文献(reference)

Autosar Guidelines C++14 example code compile list(1-169)
https://qiita.com/kaizen_nagoya/items/8ccbf6675c3494d57a76#_reference-3a2b9cfd1b05f6a444c2


Autosarの課題
https://qiita.com/kaizen_nagoya/items/617d10b0e34143030600

英語(1) プログラマが知っているとよい英単語の語源
https://qiita.com/kaizen_nagoya/items/9de6d47c47e2c211222b

#文書履歴(document history)
ver. 0.01 初稿 20200119 
ver. 0.02 URL追記 20200120

<a href="https://b.hatena.ne.jp/entry/s/qiita.com/kaizen_nagoya/items/5f547173544703d267aa" class="hatena-bookmark-button" data-hatena-bookmark-layout="basic-label-counter" data-hatena-bookmark-lang="ja" title="このエントリーをはてなブックマークに追加"><img src="https://b.st-hatena.com/images/v4/public/entry-button/button-only@2x.png" alt="このエントリーをはてなブックマークに追加" width="20" height="20" style="border: none;" /></a><script type="text/javascript" src="https://b.st-hatena.com/js/bookmark_button.js" charset="utf-8" async="async"></script>

https://b.hatena.ne.jp/guide/bbutton
