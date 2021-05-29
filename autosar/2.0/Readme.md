Autosar 2.0を読む
https://qiita.com/kaizen_nagoya/items/b44a1047c2c517d522fe

AUTOSAR can OSEK OS 通信 

Autosarについて、背景を理解すれば、すごくわかりやすいことがある。

Autosar 2.0は、最初の公開仕様である。その一部をOpen souceとして作成事業に携わってきた。
https://www.toppers.jp/osek-os.html

現在でも、廃止になっていない仕様は、2.0版を公開している。

#文書入手(document download)
https://www.autosar.org/nc/document-search/

![document search.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/51423/cccca84c-4398-a7d7-6402-ee1ee0da0d4f.png)

Classic Platformの
Releaseの
06.2006 2.0.1
の左だけレ点を入れ、
それ以外のレ点を外し、
「search」を押す。

なぜか、一度に全部のダウンロードをしようとするとシステムが反応しない。
少なくとも２回に分けてダウンロードする必要がある。

残念なのは、廃止になった仕様は、過去の仕様を非公開にしていることだ。
どういう仕様が、どういう問題だからなくなったのかが、わからないと、
同じ間違いを繰り返すかもしれない。

# 文書属性

大きく分けて、
Requirementという名の仕様と、
Specificationという名の仕様がある。
それ以外は、仕様を理解するのに役立つ資料。


|filename|category|pdf|
|:----|:----|:----|
|AUTOSAR_MainRequirements.pdf|Requirements|1|
|AUTOSAR_RS_ECU_Configuration.pdf|Requirements|1|
|AUTOSAR_RS_FeatureDefinition.pdf|Requirements|1|
|AUTOSAR_RS_GraphicalNotation.pdf|Requirements|1|
|AUTOSAR_RS_InteractionBehavioralModels.pdf|Requirements|1|
|AUTOSAR_RS_InteroperabilityAuthoringTools.pdf|Requirements|1|
|AUTOSAR_RS_SoftwareComponentTemplate.pdf|Requirements|1|
|AUTOSAR_SRS_ADC_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_CAN.pdf|Requirements|1|
|AUTOSAR_SRS_COM.pdf|Requirements|1|
|AUTOSAR_SRS_Diagnostic.pdf|Requirements|1|
|AUTOSAR_SRS_DIO_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_EEPROM_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_FIM.pdf|Requirements|1|
|AUTOSAR_SRS_Flash_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_FlexRay.pdf|Requirements|1|
|AUTOSAR_SRS_Gateway.pdf|Requirements|1|
|AUTOSAR_SRS_General.pdf|Requirements|1|
|AUTOSAR_SRS_GPT_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_ICU_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_IOHW_Abstraction.pdf|Requirements|1|
|AUTOSAR_SRS_IPDUM.pdf|Requirements|1|
|AUTOSAR_SRS_LIN.pdf|Requirements|1|
|AUTOSAR_SRS_MCU_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_MemHw_AbstractionLayer.pdf|Requirements|1|
|AUTOSAR_SRS_MemoryServices.pdf|Requirements|1|
|AUTOSAR_SRS_ModeManagement.pdf|Requirements|1|
|AUTOSAR_SRS_OS.pdf|Requirements|1|
|AUTOSAR_SRS_PORT_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_PWM_Driver.pdf|Requirements|1|
|AUTOSAR_SRS_RAM_Test.pdf|Requirements|1|
|AUTOSAR_SRS_RTE.pdf|Requirements|1|
|AUTOSAR_SRS_SPAL_General.pdf|Requirements|1|
|AUTOSAR_SRS_SPI_HandlerDriver.pdf|Requirements|1|
|AUTOSAR_SRS_Watchdog_Driver.pdf|Requirements|1|
|AUTOSAR_SWS_ADC_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_BSW_Scheduler.pdf|Specifications|1|
|AUTOSAR_SWS_C_ImplementationRules.pdf|Specifications|1|
|AUTOSAR_SWS_CAN_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_CAN_Interface.pdf|Specifications|1|
|AUTOSAR_SWS_CAN_TP.pdf|Specifications|1|
|AUTOSAR_SWS_CAN_TransceiverDriver.pdf|Specifications|1|
|AUTOSAR_SWS_COM.pdf|Specifications|1|
|AUTOSAR_SWS_ComManager.pdf|Specifications|1|
|AUTOSAR_SWS_CompilerAbstraction.pdf|Specifications|1|
|AUTOSAR_SWS_ComStackTypes.pdf|Specifications|1|
|AUTOSAR_SWS_CRC_Routines.pdf|Specifications|1|
|AUTOSAR_SWS_DCM.pdf|Specifications|1|
|AUTOSAR_SWS_DEM.pdf|Specifications|1|
|AUTOSAR_SWS_DET.pdf|Specifications|1|
|AUTOSAR_SWS_DIO_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_ECU_StateManager.pdf|Specifications|1|
|AUTOSAR_SWS_EEPROM_Abstraction.pdf|Specifications|1|
|AUTOSAR_SWS_EEPROM_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_FIM.pdf|Specifications|1|
|AUTOSAR_SWS_Flash_EEPROM_Emulation.pdf|Specifications|1|
|AUTOSAR_SWS_FlexRay_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_FlexRay_Interface.pdf|Specifications|1|
|AUTOSAR_SWS_FlexRay_TP.pdf|Specifications|1|
|AUTOSAR_SWS_FlexRayTransceiver.pdf|Specifications|1|
|AUTOSAR_SWS_GPT_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_ICU_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_IOHWAbstraction.pdf|Specifications|1|
|AUTOSAR_SWS_IPDUM.pdf|Specifications|1|
|AUTOSAR_SWS_LIN_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_LIN_Interface.pdf|Specifications|1|
|AUTOSAR_SWS_MCU_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_Mem_AbstractionInterface.pdf|Specifications|1|
|AUTOSAR_SWS_MemoryMapping.pdf|Specifications|1|
|AUTOSAR_SWS_NVRAM_Manager.pdf|Specifications|1|
|AUTOSAR_SWS_OS.pdf|Specifications|1|
|AUTOSAR_SWS_PDU_Router.pdf|Specifications|1|
|AUTOSAR_SWS_PlatformTypes.pdf|Specifications|1|
|AUTOSAR_SWS_Port_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_PWM_Driver.pdf|Specifications|1|
|AUTOSAR_SWS_RAM_Test.pdf|Specifications|1|
|AUTOSAR_SWS_RTE.pdf|Specifications|1|
|AUTOSAR_SWS_SPI_HandlerDriver.pdf|Specifications|1|
|AUTOSAR_SWS_WatchdogDriver.pdf|Specifications|1|
|AUTOSAR_SWS_WatchdogInterface.pdf|Specifications|1|
|AUTOSAR_SWS_WatchdogManager.pdf|Specifications|1|
|AUTOSAR_BasicSoftwareModules.pdf| |1|
|AUTOSAR_DS_CT_Path_D.pdf| |1|
|AUTOSAR_ECU_Configuration.pdf| |1|
|AUTOSAR_FeatureDefinition.pdf| |1|
|AUTOSAR_Glossary.pdf| |1|
|AUTOSAR_GraphicalNotation.pdf| |1|
|AUTOSAR_InteractionBehavioralModels.pdf| |1|
|AUTOSAR_InteroperabilityAuthoringTools.pdf| |1|
|AUTOSAR_LayeredSoftwareArchitecture.pdf| |1|
|AUTOSAR_Methodology.pdf| |1|
|AUTOSAR_ModelPersistenceRulesforXML.pdf| |1|
|AUTOSAR_SimulinkStyleguide.pdf| |1|
|AUTOSAR_SoftwareComponentTemplate.pdf| |1|
|AUTOSAR_TechnicalOverview.pdf| |1|
|AUTOSAR_TemplateModelingGuide.pdf| |1|
|AUTOSAR_TemplateModelingPatterns.pdf| |1|
|AUTOSAR_UML_Profile.pdf| |1|
|AUTOSAR_MetaModel.zip|Autosar_metamodel.eap| |
|AUTOSAR_Schema.zip|Autosar..xsd| |
|Main.zip|3| |
|MethodologyAndTools-02Template.zip|5| |
|MethodologyAndTools-Methodology.zip|2| |
|MethodologyAndTools-Tools.zip|10| |
|SW_Architecture-Communication_Stack.zip|21| |
|SW_Architecture-Diagnostic_Services.zip|6| |
|SW_Architecture-General.zip|3| |
|SW_Architecture-Implementation_Integration.zip|4| |
|SW_Architecture-Memory_Stack.zip|12| |
|SW_Architecture-Peripherals.zip|22| |
|SW_Architecture-RTE.zip|2| |
|SW_Architecture-System_Services.zip|7| |
| |97| |

困ったことは2つ

1. 一括ダウンロードがエラーになる。
2. Zipファイルの中にも、文書が入っていて重複ダウンロードになる。

#  項目
2006年の2.0と2020年の20-11で、項目が激変している。

一番大きいのはinitiator（提案者）。
誰が言い出したかわかる仕様は、とても役に立つ。
必要性も理解しやすい。
複数の仕様で、他の人が言っていることなら、
選択的な並列な仕様かもしれないことも分かる。



項目|2.0|(20-11|説明|
|:----|:----|:----|:----|
|Initiator|1| |提案者|
|Date|1| |日付|
|Autosar Release|1| |対応版|
|Short description|1| |概要|
|Type|1|1|型|
|Importance|1| |重要性|
|Description|1|1|説明|
|Rationale|1| |根拠|
|Use Case|1|1|事例|
|Dependencies|1|1|依存|
|Conflicts|1| |制限|
|Supporting material|1|1|支援事項|

こんなに項目が減っている。たとえば、同じ内容を規定しているBSW00342を次に示す。


## autosar 2.0
![bsw.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/51423/36aa27bc-cee6-62de-f760-00e5b705a949.png)
![bsw2.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/51423/c2d83256-5283-76d0-e85b-78838fc56d7f.png)

## autosar '20-11
![bsw3.png](https://qiita-image-store.s3.ap-northeast-1.amazonaws.com/0/51423/0600477d-9feb-9956-8236-4515aa2429d3.png)

AUTOSAR 2.0を読むと、AUTOSARを理解できる。


# Model Based Design

Autosar 2.0は、Autosarが目指していた方向性を理解するのによい。

Applying Simulink to AUTOSARでは、
モデルベース開発から全ソフトウェアを自動生成するための道筋を検討している。


Scope

>This document is concerned with describing the elements that constitute an AUTOSAR software component in Simulink. Given this “mapping” of the component structure it is possible to use Simulink to describe the behavior of individual control mod- ules, for application with a code generator to create implementations that are harmonized with the AUTOSAR RTE, and to create system wide simulators of the entire ECU network and physical environment.
In this document, Simulink will be considered in the role of a behavior modeling tool rather than an AUTOSAR authoring tool.

仮訳
「この文書は、SimulinkのAUTOSARソフトウェア部品を構成する要素を説明しています。 部品構造の「対応づけ」を考えると、Simulinkを使用して個々の制御モジュールの動作を記述したり、コード生成器を使用してAUTOSAR RTEと調和する実装を作成したり、システム全体のECUネットワーク全体と物理環境シミュレータを作成します。 
この文書では、Simulinkは、AUTOSAR制作器ではなく、動作モデリング器の役割です。」

なぜうまくいかなかったかは推測しかできない。Matlabの開発元であるMathworksの協力が得られなかったのか、Mathworksとの連携が嫌な会社があったのかはわからない。

#背景

## 排ガス規制
自動車用計算機制御は、本田の排ガス規制で一躍注目を浴びた。

語り継ぎたいことトップ>Hondaのチャレンジングスピリット>CVCCエンジン発表 / 1972
https://www.honda.co.jp/50years-history/challenge/1972introducingthecvcc/

制御装置以外の装置を使うのではなく、新しい材料を使うのではなく、
費用対効果が抜群だったのだろう。

その後、MATLABなどのモデルから自動生成するのが流行ってきた。
AUTOSARの基本も制御モデルから始まる。

ちなみに、1972年は、現在のPCの基本機能を構成する技術である4004, C言語とEthernetが始まった頃らしい。
詳しくは、4004は1971年。
https://www.intel.co.uk/content/www/uk/en/history/museum-story-of-intel-4004.html
C言語はStephen C. JohnsonがPortable C Compilerとして提供し、GCCが主流になるまで続いた。
https://citeseer.ist.psu.edu/viewdoc/download?doi=10.1.1.48.3512&rep=rep1&type=pdf
ちなみに、S.C Johnsonは、その後Matlab Compilerに関してMathworksに入っている。
https://www.usenix.org/legacy/publications/library/proceedings/vhll/full_papers/vhll94_paper_johnson.pdf

Ethenetが実用化したDIX仕様は1980年である。
https://ethernethistory.typepad.com/papers/EthernetSpec.pdf

いかに、ホンダのエンジン制御が歴史があるかが分かる。

## 安全
排ガス規制を達成しても、自動車が安全でなければ意味がない。
電子制御が危険の原因を作らないことが大切である。

##省エネ
電気自動車では、排ガス規制は関係がない。
走行距離と燃費が大事だ。
そのためには、電池の容量と重さ、大きさが重要である。
また、電動機の出力と効率が大事だ。
ここでも、計算機制御の能力がとても大事。

## 通信
排ガス規制を達成し、安全で省エネな計算機制御を実現するには、
安全で省エネな通信系が必要である。
Controller Area Network(CAN)は、電気的に調停を行うため、
無駄な通信を防ぎ、計算機に負荷をかけずに効率的な通信を行うことができる。
##基本ソフトウェア
制御だけであれば、Operating System(OS)は必要ない。
通信を利用した制御を行うには、
制御の邪魔をしないで、通信を助けるOSがあるとよい。

OSEKは、割り込みでエンジン・電動機制御処理を行い、タスクはエンジン・電動機制御処理をじゃましないように、通信を助けるようにする。

https://www.irisa.fr/alf/downloads/puaut/TPNXT/images/os223.pdf

## ソフトウェアによる設計

ハードウェアができてからソフトウェアを開発始めるのでは競争に勝てない。その意味で、AUTOSARは競争領域である。

そこがAUTOSARがうまく機能していない理由かもしれない。

## バベルの塔

基本設計の方針が、下の方と、上の方で一貫性がないといけない。
時間制約を下から上まで一貫性がないと、機能しないことがわかっていない人が関与したのかもしれない。

下の層でPORTと呼んででいるPort Driverは、物理的なピンを指す。
AUTOSARの文書では、上の層でPORTと呼んでいるのは、記述によっては、rte portという用語も出てくるが、portとだけ書いてソフトウェア部品の通信の入出力を指している。

機能は類似である。一般用語としては、ありである。技術用語としては、ハードウェアとソフトウェアで同じ名前では困る。

技術用語であれば、port, software portとするか、
hardware port, portとするか
hardware port, software portとするかの
３択で、両方portと呼ぶのは止めて欲しい。

Signal, Channelなども同じように、ハードウェアとソフトウェアで別のものを指している。

AUTOSARはバベルの塔になっているかもしれない。

＜この記事は個人の過去の経験に基づく個人の感想です。現在所属する組織、業務とは関係がありません。＞
