「自動車の故障診断に関連するプログラマーになりたての方が参照するとよさそうな情報」の読み方
https://qiita.com/kaizen_nagoya/items/0c6b8373f93ce52def33

は、@kazuo_reve さんの
「自動車の故障診断に関連するプログラマーになりたての方が参照するとよさそうな情報」
https://qiita.com/kazuo_reve/items/f773b320dcbf2ab316da

に基づいている。

ここでは、いくつかの大事な記事を参照している。
その一つが、

MONOistの「AUTOSARを使いこなす」の連載記事一覧。櫻井剛さんが執筆。
AUTOSARを使いこなす
https://monoist.atmarkit.co.jp/mn/series/9343/

今回は、そのうちの一つの記事を取り上げる。
ただし、先頭に掲げた２つの記事を読んでいる人を対象にし、法律、条約について理解していることを前提とする。

自動車の“安全”を考える、ISO 26262の先にある「SaFAD」にどう対応すべきか
https://monoist.atmarkit.co.jp/mn/articles/2008/27/news008.html

役立つのが参考文献。

>参考文献（順不同）
［1］ISO 26262:2018 Road vehicles - Functional safety (all parts)
［2］ISO/PAS 21448:2019 Road Vehicles - Safety of the intended functionality (SOTIF)
［3］Safety First for Automated Driving (SaFAD paper) (2019-07)
https://www.daimler.com/documents/innovation/other/safety-first-for-automated-driving.pdf
［4］国土交通省自動車局 自動運転車の安全技術ガイドライン (2018-09-12)
https://www.mlit.go.jp/common/001253665.pdf
［5］ACEA Strategy Paper on Connectivity (2016-04)
［6］伊藤: 自動車データ活用に関する欧州の動向 JARI Research Journal (2018-05-01)
［7］自動走行ビジネス検討会 自動走行システムにおけるサイバーセキュリティ対策 (2019-06-26)
［8］AV: Bringing Standards Together for Safety, EE Times Asia (2020-04-21)

また、節構成が規格になっている。

>1．ISO 26262 Road vehicles - Functional safety
2．ISO/PAS 21448:2019 Road Vehicles - Safety of the intended functionality（SOTIF）
3．ISO 20077 Road Vehicles - Extended vehicle (ExVe) methodology
4．ISO/SAE 21434 Road Vehicles - Cybersecurity engineering
5．SAE J3061_201601 Cybersecurity Guidebook for Cyber-Physical Vehicle Systems (2016-01-14)


大事なのは、基本発想。

SaFADは、ISO 26262の先にあるのではない。
ISO 26262は、自動車安全の一つの分岐である。
SoTifもSaFadも自動車安全の分岐である。
ISO 26262の分岐ではないことを想定した方が理解が早いかもしれない。

じゃ、自動車安全はどこに規格があるのだという疑問が湧くかもしれない。

安全に関する規格の基本は、Guide 50, Guide 51.

ISO/IEC GUIDE 50:2014
Safety aspects — Guidelines for child safety in standards and other specifications
https://www.iso.org/standard/63937.html


ISO/IEC GUIDE 51:2014
Safety aspects — Guidelines for their inclusion in standards
https://www.iso.org/standard/53940.html

課題は、機械安全が隔離の原則という危険源からの距離で安全を確保しようとするのに対し、自動車安全は危険源の中に人間がいるという状況でどう安全を確保するかである。
そのため、自動車安全は機械安全の下にはない。

機能安全規格は、機械安全規格を助けるための電気・電子の安全規格であり、自動車安全には直接的に貢献するかどうかは、統計的なデータをまだ探しきれていない。

Functional safety of electrical/electronic/programmable electronic safety-related systems 
https://webstore.iec.ch/publication/22273
