# 職務経歴書

## 基本情報

| key | value |
|:---:|:------|
| 氏名 | 佐藤 壮一（Soichi Sato） |
| 生年月日 | 1989-01-21 |
| 居住地 | 秋田県 |
| 出身地 | 青森県 |
| 最終学歴 | 東北大学大学院工学研究科通信工学専攻 |

## 各種アカウント

<p>
<a href="https://github.com/Soh1121" target="_blank"><img alt="Github" src="https://img.shields.io/badge/-Soh1121-181717.svg?logo=github&style=popout" /></a>
<a href="https://twitter.com/soh_1121_" target="_blank"><img alt="Twitter" src="https://img.shields.io/badge/-soh_1121_-1DA1F2.svg?logo=twitter&style=popout&logoColor=white" /></a>
<a href="https://qiita.com/Soh1121" target="_blank"><img alt="Qiita" src="https://img.shields.io/badge/-Soh1121-55C500.svg?&logo=qiita&style=popout&logoColor=white" /></a>
<a href="https://zenn.dev/soh1121" target="_blank"><img alt="Zenn" src="https://img.shields.io/badge/-soh1121-3EA8FF.svg?&logo=zenn&style=popout&logoColor=white" /></a>
</p>

## 資格

| 取得年月 | 資格名 |
|:-------:|:------|
| 2012年11月 | 基本情報技術者試験 合格 |
| 2014年9月 | 第一級陸上無線技術士 取得 |
| 2019年6月 | 応用情報技術者試験 合格 |
| 2019年12月 | AWS Certified Cloud Practitioner 合格（失効） |
| 2020年3月 | AW㻿 Certified 㻿olution Architect - Associate 合格（失効） |
| 2021年3月 | AWS Certified Developer - Associate 合格（失効） |
| 2024年12月 | 情報処理安全確保支援士試験 合格 |

## 保有スキル

- PHP＋Laravelでのバックエンド開発・設計・テスト
- Go言語でのバックエンド開発・設計・テスト
- DDDを意識したクラス設計
- Pytonでの自然言語処理
- 要件定義・設計から結果の評価・分析までの一気通貫したアプリケーション開発
- AWSを用いた可用性の高いアーキテクチャ設計・構築

## 技術スタック

### 言語

<p>
	<img alt="PHP" src="https://img.shields.io/badge/-PHP-777BB4.svg?logo=php&style=popout&logoColor=white" />
	<img alt="Go" src="https://img.shields.io/badge/-Go-555.svg?logo=go&style=flat" />
	<img alt="Python" src="https://img.shields.io/badge/-Python-3776AB.svg?logo=python&style=popout&logoColor=white" />
	<img alt="JavaScript" src="https://img.shields.io/badge/-JavaScript-F7DF1E.svg?logo=javascript&style=popout&logoColor=white" />
</p>

### フレームワークなど

<p>
	<img alt="Laravel" src="https://img.shields.io/badge/-Laravel-FF2D20.svg?logo=laravel&style=popout&logoColor=white" />
	<img alt="pandas" src="https://img.shields.io/badge/-pandas-150458.svg?logo=pandas&style=popout&logoColor=white" />
	<img alt="Docker" src="https://img.shields.io/badge/-Docker-2496ED.svg?logo=docker&style=popout&logoColor=white" />
	<img alt="AWS" src="https://img.shields.io/badge/-AWS-232F3E.svg?logo=amazonaws&style=popout&logoColor=white" />
</p>

## 職務経歴詳細

### 株式会社ホワイトプラス【2023/05〜現在】

宅配クリーニングサービスにおいて、クリーニング工場で使用するWebシステムの開発・運用・保守に従事。  
注文を受け付ける際の最適な工場の割り当てや、クリーニング・保管・発送工程における管理機能の開発が主な担当業務。  

#### PHPバージョンアッププロジェクト【2023/05〜2025/03】

##### 概要

PHP 7.4・Laravel 6からPHP 8.2・Laravel 10へバージョンアップするプロジェクト。  
バージョンアップに伴い、abandonedとなったパッケージの移行や非同期処理基盤の構築も行った。

##### 体制

メンバーの1人として参画。

- EM：1名
- プロジェクトリーダー：1名
- メンバー：3名
- 業務委託：3名

##### 使用技術

- PHP（7.4・8.2）
	- PHPStan
- Go（1.24）
	- gomock
	- golangcli-lint
	- air
- GCP
	- Cloud Run
	- Cloud Run Jobs
	- Cloud Run Functions
	- FireStore
	- Cloud Storage
	- Cloud Build
	- Cloud Deploy
	- Pub/Sub
	- Eventarc
	- Workflows
	- Cloud Scheduler
	- Cloud Logging
	- Cloud Monitoring
	- Cloud Trace
	- IAM
- Terraform

##### 担当業務

- PHPStanのカスタムルールの作成
	- 非互換な変更をPHPStanを用いて検出
- 非互換な変更の修正対応
	- PHPStanにより検出されたものを修正
	- 型推論が機能せず疑陽性となった部分は型宣言・型情報を追加
	- 実際に非互換な変更により動かなく部分はリファクタリングを実施
- [`laravelcollective/html`](https://packagist.org/packages/laravelcollective/html) から [`spatie/laravel-html`](https://packagist.org/packages/spatie/laravel-html) への移行
	- 対象箇所：約1,700箇所
	- 移行ツール [SHIFT](https://laravelshift.com/convert-laravelcollective-html-to-spatie-laravel-html) を使用した移行
	- 移行できなかった部分の修正
	- 意図しない形へ書き換えられていた部分の修正
- 非同期処理基盤の構築
	- 主にレビュアーとしてGoでの実装のレビュー、Terraformのレビューを実施
	- 部分的にGCPリソースの作成、実装の修正も担当
	- 処理状況をクライアント側で確認する検索画面の作成
- 業務委託のハンドリング
	- 非互換な変更の修正対応の指示出し・レビュー
	- 修正方針の検討・調整

##### 工夫した点

- ツールによる一括変換により大幅な時間短縮を図るとともに、意図しない変換を精査し、短時間で一定の品質でパッケージを移行した
- Terraformの知見が少なかったが、基礎をキャッチアップしてから取り組むことでレビュー品質の向上につながった
- ドキュメントを整えることで、外注メンバーとの連携・レビュー体制を整備し、全体の開発効率・品質を両立した

### 株式会社ラクス（株式会社ラクスライトクラウド出向）【2022/01〜2023/04】

メール配信エンジンSaaSのblastengineにおいて、アカウント情報管理APIの開発・運用・保守に従事。  
別システムとの連携も踏まえながら、ユーザーの利便性を高める追加機能の設計からリリースまで実施。  
ドメイン駆動設計を部分的に導入して、変更容易性を高めるよう努めた。

#### プロジェクト規模

- 企画：2名
	- サービスの仕様検討
- サポート：1名
	- 業務フローの確認
- 開発：4名
	- エンジニアリングマネージャー1名：退職により7月末に離脱
	- フロントエンドエンジニア1名
	- バックエンドエンジニア2名
		- アカウント情報管理API：1名（★自身が担当）
		- メール配信エンジンAPI：1名

#### 使用技術

- PHP 7.4
	- PHPUnit
	- PHPStan
	- Mockery
- Laravel 7.x
- Docker
- Docker Compose
- MongoDB
- GitLab

##### 取り組み

###### DDDを用いた設計への移行

DDDを学習し、値オブジェクトやモデルなどを用意することで、処理の集約を目指した。  
テストに関しては、UseCase層のInterfaceやモックを用意して、差し替えて異常系のテストも行えるようにした。

###### モックサーバーを用いたI/Fの認識合わせ

先に開発が進んでいた別システムとの連携では、I/Fの認識のずれによる修正がたびたび発生していた。  
そのため、フロントエンドとのI/Fに関してはあらかじめ認識を合わせて実装するため、Swaggerを用いて簡易なモックサーバーを構築したうえで実装した。

### 日本放送協会【2013/04〜2021/12】

番組制作・設備整備・イベントの企画運営・研究開発など、非常に幅広い業務に従事。

#### 営業局IT営業推進部【2021/07〜2021/12】

##### 概要

営業システムの整備業務に従事。  
オンプレミスのシステムの定期保守や入れ替えの仕様決め、クラウド移行のための運用ルールの策定などを行った。  
クラウドやGitなど、Web開発に必要な知識を持っているメンバーが少ない中で、資料の作成や勉強会を通してメンバーのスキルアップに努めた。

#### 放送技術研究所ネットサービス基盤研究部【2018/08〜2021/06】

##### 概要

教育分野では超スマート社会「Society5.0」に向けた「学校ver.3.0」が提案され、個別最適化された学びが注目を集めている。  
関連する映像コンテンツ提示の際に、コンテンツ同士の関連性を提示することが学びの個別最適化につながることがわかっていた。  
そこで、関連性を自動推定するためのナレッジベースを構築し、これを組み込んだ関連コンテンツレコメンドシステムを発注して試作。  
実際に学生に利用してもらい、ナレッジベースによる関連コンテンツ提示を評価した。

##### 担当

- ナレッジベースの構築
- レコメンドシステムの要件定義・設計
- 実証実験の実験設計・分析／評価

##### 使用技術

- Python
	- pandas
	- numpy
	- scikit-learn
	- matplotlib
	- gensim（word2vec）
- RDF（Resource Description Framework）：主語・述語・目的語の3つ組で情報を表すデータ構造
	- Turtle：ファイル形式
- SPARQL：RDF用のクエリ言語
- MeCab：形態素解析器

##### 課題

- ユーザー情報を用いない内容ベースのフィルタリングを構築する必要がある
- 学校教育の学習内容をデータ化したものが存在しない
- 既存のナレッジベースではナレッジベースから関連するデータを抽出した後、機械学習などを用いて関連性の強さを測る必要がある
- コロナ禍で実験室実験が行えない

##### 取り組み

###### ナレッジベースの構築

単語と単語の関連性を定義（上位・下位概念や因果関係など）し、その関連性の強さをword2vecを用いて数値化。  
それらをRDFというデータ構造のTurtle形式でナレッジベースとして構築した。

##### Webアプリケーションとしてレコメンドシステムの要件定義・設計

実証実験を行うためのレコメンドシステムを試作するにあたり、要件定義・基本設計を担当した。  
コロナ禍では、実験室実験が行えないため、これまでの実験はサーバーを実験室に持ち込んでシステム構築していたが、Webアプリケーションとして構築することとした。

##### 実験評価・分析

ユーザーを2つのグループに分け、関連コンテンツ抽出アルゴリズムをそれぞれ別のものを用いてユーザーに関連コンテンツを提示。  
ナレッジベースを用いた関連コンテンツ提示アルゴリズムの有効性を検証・分析した。

##### 工夫した点

- 教科書をテキストデータ化し、学校教育の学習内容をデータ化するための学習データとして用いた
- RDFで関連性のみを定義するのではなく、関連性の強さも定義することでナレッジベースの利用者は後段で機械学習を用いずともレコメンドなどを行えるようにした

#### 報道局社会番組部【2017/08〜2018/07】

##### 概要

参加者が番組を企画するアイデアソン『ディレクソン』の企画・運営に従事。  
イベント開始前から終了後まで参加者をフォローアップするコミュニティーの運営に力を入れ、参加者とNHKをつなぐファンマーケティングにつながるよう努めた。

#### 秋田放送局技術部【2013/05〜2017/07】

##### 概要

番組制作や設備整備、放送送出など幅広い業務に従事。  
地方局では数少ないデータ放送コンテンツ制作に注力し、スポーツ中継におけるTwitterを用いた応援メッセージの紹介や、人口減少などの地域にちなんだ問題に対する討論番組でのアンケートの実施などを行った。

一例として、プロバスケットボールbjリーグ（現Bリーグ）における応援合戦コンテンツを紹介する。  
この取り組みはTwitterやメールフォームを通じて両チームへの応援メッセージを募集し、寄せられたメッセージの数をリアルタイムでデータ放送上に表示して競い合うコンテンツだった。

##### 担当

- 提案
- 実施交渉
- 設計
- データ放送コンテンツ制作
- メッセージ数集計スクリプト作成
- データ放送コンテンツ送出
- 実施後の振り返り

##### 使用技術

- BML（Broadcast Markup Language）
- ECMAScript
- Ruby

##### 課題

- 応援コンテンツはメッセージ投稿募集型かボタン連打型の2種類のみだった
- 自チームの応援メッセージのみを募集しても寄せられる数は限られていた
- 秋田放送局・富山放送局両局で放送するインターローカルという放送形式で、データ放送コンテンツを送出するうえで実施交渉の難易度が高かった

##### 取り組み

###### 提案から振り返りまで一気通貫で担当

提案から振り返りまで、主にひとりで担当し完遂した。  
特にスポーツ中継は生放送故に、放送して実績を出したらそれで終わりということが多かった。  
しかか、どのように改善すればより盛り上がるコンテンツとなるか、メッセージ数を増やせるかなどの振り返りを実施するところまで行った。

###### 新しい応援のかたちを実現

これまでの2種類（メッセージ紹介・ボタン連打）とは異なるコンテンツの提供に成功した。  
寄せられたメッセージの数は全国放送と同等の数が寄せられ、地方局が送出した番組の中では群を抜いた数だった。
