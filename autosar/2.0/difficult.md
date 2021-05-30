AUTOSAR わかりにくいこと 10を開催します。

2004年頃から、AUTOSARを仕事で扱って、これまで約数千の質問をいただいて来ました。

半分以上が答えられていないかもしれません。
半分以上が嘘の答えをしたかもしれません。

ここでは、その反省に立って、答えられなかったり、嘘の答えをいった背景、状況、流れを記載してみます。

#0. 自然言語で記述
一部、UML、XMLなどでの記述があります。
仕様のほとんどを自然言語で書いています。

状態遷移をすべてUMLで記載していれば、まだよかったかもしれません。自然言語で記述し、仕様記述言語で書いてないAUTOSARのわかりにくさを代表するかもしれません。

文書として、Templateを作って内容を記述したり、
Metamodelを作ってModelを記述したりという仕組みはいろいろ作られています。
しかし、Templateを作って記述した内容の用語定義が整合性がなかったり、参考文献の整合性がなかったりしていては、見た目だけを揃えたということになってしまったかもしれません。

卒業研究は制御理論の研究室でモデル記述とその数値解析は得意でした。メタモデルは書いたことがなく、何のためにメタモデルを書くのかをりかいしていません。Metamodelは、実際のModel例がたくさんあれば、そのMetamodelの良さが確認しやすいかもしれません。Metamodelだけあって、実際のModel例がないと嬉しくないかもしれません。


#1. 競争領域と協力領域

何が競争領域かは、日々変わっていきます。
合意で決められるものではないという経験則があります。

相手を出し抜くことが競争なのかもしれません。
全員が合意しても、破ったときの罰則条項以上の利益があれば、
合意を破るのが経済原則ではないのでしょうか。

例えば、OEM（自動車製造・販売業）だけでも、事前に何が協力領域で、何が競争領域かを決められません。
OEM（自動車製造・販売業）と部品製造業の間では、さらに複雑で競争領域と協力領域は日々変化する可能性があります。

OEMと部品製造業と半導体会社の間は、もっと複雑でしょう。

さらに、モデル記述するMatlabのモデルからコード生成を提供する Mathworks, 
CANの通信シミュレータCANoeを提供するvector,
UMLからコード生成するEnterPrise Architectを提供するSparxsystemsなどのツールベンダ間および顧客間には、もっともっと複雑な利害関係が存在しているかもしれません。

#2. XMLは銀の弾丸か

Microsoft Excel, Wordが、OOXMLという共通の形式で記述し、
容易にC#などのプログラミング言語で扱えるようになったのは、
驚異的な変革だったかもしれません。

ISO/IEC 29500-1:2008
Information technology — Document description and processing languages — Office Open XML File Formats — Part 1: Fundamentals and Markup Language Reference


それは、Open Officeというライバルが、OpenDocumentという仕様を国際規格にして普及を促進しようとしたことへの対抗だったから成功したのかもしれません。
https://www.openoffice.org/ja/

ISO/IEC 26300:2006
Information technology — Open Document Format for Office Applications (OpenDocument) v1.0

このように、XMLは、Open化の標準化にとっては、中心的な役割を果たして来たと言えるかもしれません。

XML系のソフトウェアでは、編集作業中の整合性の確認には時間がかかりすぎること、複雑な定義ができるだめ無駄そうなデータを削ってもいいかどうかの判断が難しいこと、その結果、見た目には同じにみえるが内部でのデータの違うファイルの種類が数限りなくできる可能性があることなど、さまざまな課題があるかもしれません。

それに対して、json形式という単純なデータ構造は、
単純であるために整合性の確認に時間がかからず、
複雑な定義をしなくても処理が可能であることが習慣化し、
その結果、見た目とデータがそんなに乖離しないような気になる利点があるかもしれません。

XMLという選択はよい選択だったはずなのですが、
簡単な構造でよいものは簡単な構造にもできるという選択肢が
あってもよかったかもしれません。

#3. 一意な定義か並列な定義か

ver. 2.0では、initiatorという提案者の名前を掲載するようにしていました。そのため、複数の提案者が別の仕様を提案していれば、一意な定義ではなく並列な定義であることはとても理解しやすかったような気がします。

その後、initiatorという項目を無くしてしまい、
定義が一意か並列かがわかりにくくなっています。

#4. OSと通信規約の対応
CANとOSEKは、共存関係で発展してきました。
ちょうど, Ethernet, TCP/IP, UNIX(Linux)が発展してきたのと同じように。
FlexRayも、TTOSのような時刻同期に基づいたOSが提供できれば、
うまくいったかもしれません。

AUTOSARのAdaptive PlatformとしてEthernet, TCP/IP, UNIX(linux)を採用したように。

# 5. ISO, IEC, ITUとの関係

WTO/TBT協定に基づき、国際的な技術仕様は、ISO,IEC,ITUの文書として発行することが基本的な行動様式になっています。

AUTOSARが始まった以降に、LIN, FlexRayはそれぞれISO規格になっています。

ISO 17458-1:2013
Road vehicles — FlexRay communications system — Part 1: General information and use case definition


ISO 17987-1:2016
Road vehicles — Local Interconnect Network (LIN) — Part 1: General information and use case definition
https://www.iso.org/standard/61222.html

FlexRay Consortium, Lin Consortiumからの提案で、
AUTOSARからの提案ではなさそうです。

ISO,IEC,ITUに国際規格を協調して提案している団体は多数あります。
Liaison(連絡）関係を結びます。
例えば、IEEEは、ISO/IEC JTC1とA Liaisonを結び、
ISO/IEC/IEEEで始まる国際規格を発行しています。
IEEEでまず発行してからISO/IECに持ち込むものもあれば、
ISO/IEC/IEEEで同時に審議する場合もあります。

AUTOSARとISO,IEC,ITUとLiaison関係を確認できていません。

MISRAは、ISO/IEC JTC1/SC22/WG14などとC Liaisonを結び、
定期的に意見文書を発行しています。

MISRA C Liaison Report to ISO/IEC JTC1/SC22/WG14 21st-25th October 2019
http://www.open-std.org/jtc1/sc22/wg14/www/docs/n2445.pdf

# 6. interface

ソフトウェアDriver以外に、インタフェースというモジュールがあるらしい。interfaceといえば、モジュールとモジュールの界面(iterface)を規定するものである。インタフェースがモジュールであれば、インタフェースというモジュールのインタフェースが必要なんじゃないかと疑問に感じる人がいるかもしれない。インタフェースはモジュールにしないのがソフトウェアの仕様なのではないのだろうか。
なんでinterfaceというモジュールを作る気になったのだろう。

# 7. port, signal, channel
ハードウェアとソフトウェアで、同じ言葉を別の意味に使っている。
先頭にphysical port, rte portなど修飾語をつければ区分できる。
省略している場合は、その文書がどちらよりの文書かで判断するとよい。

# 8. 状態(state, mode)

状態をstateと読んだり、modeと読んだり、場合によってはphaseということもあるらしい。

AUTOSAR 状態遷移を網羅する(2.0版）
https://qiita.com/kaizen_nagoya/items/64535352b3f5f20e15ed

すべての状態遷移を状態遷移表(UML)で記載してみようと計画中。

# 9. ISO OSI参照

ISO OSIは、その仕様が大きすぎ、全体構造はわかるものの、それぞれの層の役割分担がわからない状態において、TCP/IPという Ethernet上の通信規約によって事実上亡き者にされたと思っていた。

AUTOSARの校正(calibration)関係の規定では、ISOのOSIをしばしば参照している。参照している文献名や発行年がいろいろ違っていて、何を参照したいかがわからないという面もある。

ISOのOSIが現代で役にたつとすれば、新たなセキュリティを強化するときの構造設計ではないだろうか。
AUTOSARの校正(calibration)がセキュリティを基盤に基本設計できているという記述は見当たっていない。ISO OSIを参照した理由がわかっていない。

#  ソフトウェア工学
ソフトウェア工学の教科書に、一人の設計者が書き下ろさないと、
よい設計にはならないという趣旨のことを書いてあったような気がする。

人月の神話―狼人間を撃つ銀の弾はない (Professional computing series (別巻3))
フレデリック・P. Jr. ブルックス
![51TWX1TAERL._SX327_BO1,204,203,200_.jpg](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/51423/e1eb0ca8-0892-3253-78bb-3d1a98b75d22.jpeg)

https://bookmeter.com/books/105264
#その他
回答しても、半分程度が記録してもらえない、口頭の質問で、回答したら結果を電子的にあとで送ってとか、GitlabのprivateのWikiに記載してと頼んで、いくつかの会社の方、技術者の方は適切に対応してくださってきました。ありがとうございます。
