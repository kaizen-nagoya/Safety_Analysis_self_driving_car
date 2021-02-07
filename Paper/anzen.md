# はじめに (c) Dr. OGAWA Kiyoshi

日本学術会議が開催している行事に、安全工学シンポジウムがあります。

共催学会は、
安全工学会
化学工学会	
火薬学会	
計測自動制御学会
自動車技術会	
静電気学会	
地域安全学会
低温工学・超電導学会
電気学会	
電気化学会	
電気設備学会	
電子情報通信学会
土木学会	
日本化学会	
日本火災学会	
日本機械学会
日本技術士会
日本計算工学会
日本原子力学会
日本建築学会（幹事学会）
日本高圧力技術協会
日本航空宇宙学会
日本材料学会	
日本信頼性学会
日本心理学会
日本船舶海洋工学会	
日本鉄鋼協会
日本人間工学会
日本燃焼学会
日本非破壊検査協会	
日本溶接協会
日本リスク学会
日本冷凍空調学会
廃棄物資源循環学会			

学会という名称でない団体の共催しています。

協賛（予定）は、
応用物理学会		
日本地震工学会		
日本経営工学会	
日本知能情報ファジィ学会		
日本デザイン学会		
日本プラントメンテナンス協会	
粉体粉末冶金協会		
日本保全学会		
日本ロボット学会	

です。プログラマに関連する学会で、共催・協賛は、
計測自動制御学会
自動車技術会	
電子情報通信学会
日本信頼性学会
日本心理学会	
日本リスク学会
日本人間工学会

共催、協賛していない学会は、
情報処理学会
日本ソフトウェア科学会
などです。

その他、著名な学会で参加していないのは、
医学係の学会と、数学・物理関係の学会と、社会科学系・人文科学系の学会です。

# 背景
2004年から、AUTOSARのopen souceの取り組みの中で、
アイシン精機さんの豊頃試験場で、試験運転実験に参加させていただき、安全工学シンポジウムでの発表題材を明確化できた。

ご指導いただいた、安全工学の専門家の方から
安全工学シンポジウムで発表するように勧められた。

以降、十数年ちょっと、合計１１回参加してきた。

今年の発表予定題材を整理する。

一人１主題を原則としており、共同研究者がほかに数人集まることを想定して３つの主題を準備する。


# AUTOSAR関連
電気自動車と自動運転を中心に、AUTOSARでまだ十分に仕様になっていない部分を洗い出し、安全に貢献するために何ができるかを整理している。

プログラマが電池設計に寄与できるプログラムを書くために
https://qiita.com/kaizen_nagoya/items/73e44e4f1ebf161f58cc

TOPPERS のAUTOSARへの貢献(更新中)
https://qiita.com/kaizen_nagoya/items/d363cf06e2176207b391

あなたの模型(Model)は離散(digital)ですか連続(analog)ですか
https://qiita.com/kaizen_nagoya/items/009b344ee145d7969d61

「風をあつめて」を計画書として事業展開してみる
https://qiita.com/kaizen_nagoya/items/92365c542714f27e5658

人間が計算機に勝てる３つのこと
https://qiita.com/kaizen_nagoya/items/49dc709d289d22846044
# MISRA C 関連

C言語規格およびC++言語規格が出るたびに、
例題を試験できる形にして、compile and go してきた。

最近はdockerを中心にgcc, clang, visual cの３種類を用いている。

MISRA C/C++, CERT C/C++も同様である。
また、AUTOSAR C++もQiitaに上げてきた。

Autosar Guidelines C++14 example code compile list(1-169)
https://qiita.com/kaizen_nagoya/items/8ccbf6675c3494d57a76

C++N4606, 2016符号断片編纂一覧(example code compile list)
Working Draft 2016, ISO/IEC 14882(1)
https://qiita.com/kaizen_nagoya/items/df5d62c35bd6ed1c3d43/


C++N4868,2018(1)3.21 expression-equivalent [defns.expression-equivalent] p5
https://qiita.com/kaizen_nagoya/items/a4487cda12d9f97c275e

OSはC++で書き直したい。その際に、C言語の#define分のマクロをC++ Templateに書き直す際に解決できていない課題がある。

C言語の#define文マクロをC++のTemplateか何かにする方法
https://qiita.com/kaizen_nagoya/items/20c3f5964cef1da037cb

[C][C++]の国際規格案の例題をコンパイルするときの課題７つ。
https://qiita.com/kaizen_nagoya/items/5f4b155030259497c4de

# HAZOP 関連

##自動運転

自動運転の安全分析
https://qiita.com/kaizen_nagoya/items/b7f4a714f6016d3c1bf3

## AUTOSAR
角速度制御によるエンジン制御、電動機制御において、
CAN通信が邪魔をしないだけでなく、
CAN通信を円滑に行うようにOSEK OSがあることを、
HAZOP分析することにより示す。

## MISRA
MISRA C/C++の規則をFMEA的な視点で分類するとともに、
HAZOPでも分類するとわかりやすくなる。

## QC検定
安全分析手法であるHAZOPを、QC検定の題材に適用し、
QC検定の内容がHAZOPを導入すれば豊富になることを提案しようとしている。

プログラマがQC検定受けることの意味・価値・課題
https://qiita.com/kaizen_nagoya/items/b03216eb6ab09eacc957


#まとめ

社名入り、社名なし

連名者あり、単独（単独の場合は１件のみ）

連名者社名あり、連名者社名なし

のいずれをも想定。

場合によっては、英語にして自動車技術会に投稿するかもしれない。（その場合の連名の可否は別途相談）

|題材|自社名あり|自社名なし|連名者なし|連名者あり|
|--:|--:|--:|--:|--:|--:|
|AUTOSAR|10|10|30|30|
|MISRA |10|10|20|20|
|HAZOP|10|10|20|20|

資料の内容が充実していくと、上記確率が上昇する予定。
連名者なしの場合は、合計が100%越えることはない。
それ以外は、対応して隣接する２つの合計が100%を越えることはない。


自分が参加した過去の目次を掲載しました。

####第37回　安全工学シンポジウム (2008)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/778165f035bc3bf3a87546d449d1fa6c?frame_id=576083


####第38回　安全工学シンポジウム(2009)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/093356c653ddda117afe695897a2cb23?frame_id=576083

https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/671def8a04af8b39b5cd96ec68acf503?frame_id=576083

####第39回　安全工学シンポジウム(2010)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/6eec73f0e2612a815dc7e8bc4d8a3602?frame_id=576083

#### 第40回　安全工学シンポジウム(2011)
標題一覧
https://researchmap.jp/multidatabases/multidatabase_contents/detail/231120/0aa49a5883ed84f300d6657f4b30ef8f?frame_id=576083

#### 第42回　安全工学シンポジウム(2013)
HAZOPと関連手法の展開
https://www.slideshare.net/kaizenjapan/hazop-anzen21013

#### 第44回　安全工学シンポジウム(2015)
 安全(safety)と安心(security)に関す るC言語コーディング標準の取組     安全工学シンポジウム2015 小川清（技術士（情報工学）・工学博士・   　 名古屋市工業研究所）
https://www.slideshare.net/kaizenjapan/study-on-safety-and-security-ccoding-standards

 安全分析において、HAZOP, FMEA, FTAの組み合わせによる リスクアセスメントの進め方の検討 HAZOP, FMEA and FTA for Risk Assessment 日本学術会議安全工学シンポジウム Tokyo, July 2, 2015 ○ 小川明秀（大同大学） 小川 清 （技術士（情報工学）・工学博士・ 名古屋市工業研究所）
https://www.slideshare.net/kaizenjapan/hazopogawa2015

#### 第45回　安全工学シンポジウム(2016)
安全工学シンポジウム（安全と安心）2016
https://researchmap.jp/blogs/blog_entries/view/82322/26d6134a86a9ea86df64be42487d821d?frame_id=445675

安全分析における HAZOP-TRIZ連携の試み
https://www.slideshare.net/kaizenjapan/hazop-and-triz-byoffor-the-children13
#### 第46回　安全工学シンポジウム(2017)
HAZOP-­‐TRIZ連携による   交通安全分析  
https://www.slideshare.net/kaizenjapan/road-traffic-safety-analysis-with-hazop-and-triz

#### 第48回　安全工学シンポジウム(2019)

https://researchmap.jp/blogs/blog_entries/view/109203/b3e2ade8d2fcb4089c66f602f316b40a?frame_id=416975&lang=en

1-4機械の制御システムの設計における安全分析の事例報告尾崎秀典，青島武志，可兒利弘，路　海寧（オプトン），○間瀬　剛，松原和音，斉藤直希，小川　清（名古屋市工業研究所）
1-5HAZOPとTRIZを適用した新製品開発とその安全分析○斉藤直希，間瀬　剛，松原和音，小川　清（名古屋市工業研究所），寺久保　敏，石津和紀，坪井俊之（システム技術研究会）
1-6医療システムへのHAZOP適用○松原和音，間瀬　剛，斉藤直希，小川　清（名古屋市工業研究所）
4-1災害支援無線系における安全分析手法の応用○小川　清，斉藤直希，間瀬　剛，松原和音（名古屋市工業研究所），村上　孝，小寺浩司（デンソークリエイト），福田仁志（豊田自動織機）
5-3安全分析の図的表現方法、及び設計文書と親和性の高いツールの提案○田中伸明（ガイオ・テクノロジー），小川　清（名古屋市工業研究所）



鍵：andean

未来（未来短歌会）月と鏡集　佐伯裕子　選　p.65 安全工学シンポジウム 　 小川清
https://researchmap.jp/blogs/blog_entries/view/78881/2af9d72857252c9112e4d98dbcca7d59?frame_id=412479

>零細な工場を安全にするため機械分析設計極める
非常時の無線連絡見直して職務で亡くなる人がなきよう
Wi-Fi（ワイファイ）の相互接続容易化にSSID(エスエスアイディ)00000JAPAN（ファイブゼロジャパン）
医療系システムオープンソースでと言ったら医師から声がかかった
各アプリ相互接続できるよう災害想定して実験す
Twitter, facebookとLineからinstagram, mastodonまで
災害が起きたらすぐに知らせるよIT技術その日のために
