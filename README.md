# 職務経歴書

2023年3月17日現在

Hajime Terasawa (@terakoya76)

1993年生まれ神奈川県在住

* Twitter `https://twitter.com/terakoya76`
* GitHub https://github.com/terakoya76
* Blog https://medium.com/@terako.studio
* Email `terako.studio(at)gmail.com`


## できること

* フロントエンド開発
  * jQuery/React.js/Vue.js等の経験
* バックエンド開発
  * Ruby/Go/Node.js等のプログラミング言語の経験
* WebアプリケーションにおけるSRE/DevOps
  * GitHub等を用いた開発プロジェクトの管理
  * Circle CI/GitHub Actions/AWS CodeBuild/Jenkins等を用いたCI環境の構築・運用
  * Circle CI/GitHub Actions/AWS CodeDeploy/Jenkins/ArgoCD等を用いたCD環境の構築・運用
  * アプリケーションをまたいだ問題解決とプロジェクト推進
  * Mackerel/NewRelic/Datadog等を用いた監視体制の構築・運用
  * SLIの決定と実装、SLOの策定
  * 障害対応およびポストモーテムの実施
  * 全体的な開発チームのサポート
* インフラ・ミドルウェアの構築・運用
  * ネットワークやインフラ技術の基礎的な知識
  * Terraform/nsibleを使ったIaCによる構成管理の環境の構築・運用
  * Docker/Kubernetesの構築・運用
  * MySQL等のRDBMSの設計・運用
  * 小規模から大規模までのAWS活用
* その他
  * GitHubやドキュメントツール、Slack等による非同期コミュニケーション
  * 職種や技術領域をまたいだ、全体最適を目指した問題解決のアプローチ、およびその推進
  * 5人規模のチームのチームビルティング、開発計画策定、技術選定、プロジェクトマネジメント


## 職務経歴

### （株）obniz

業務委託として2021年12月〜現在まで勤務（フルリモート勤務）

#### インフラチーム: インフラエンジニア

2021年12月〜

* セキュリティ投資計画策定
* 踏み台サーバの構築
  * STNS/google-authenticatorで実装
  * 後にSTNS/Cloudflare Accessへ置き換え
* 脆弱性スキャン構築・運用
* VPSベースのマイクロサービスアーキテクチャの耐障害性対応
  * nginxによるAPサーバ冗長化
  * pgpool2によるPostgreSQL HA構成構築
* バックエンドサービス群の一部AWS移行設計・実施
  * Nameserver Cloudflare移行
  * terraform導入・運用
  * 移行計画策定
  * DB単体でのAWS移行
  * AMI Build Pipeline整備
  * AP系のAWS移行
* 情報系に対するCloudflare CDN導入
* NewRelicによる監視整備

### freee（株）

2017年06月〜2022年05月の間勤務（2020年よりフルリモート勤務）
* 正社員として2017年10月〜2022年05月の間勤務
* インターンとして2017年06月〜2017年09月の間勤務


#### 基盤チーム: SRE

2019年08月〜2022年05月

* EC2ベースのRuby on Railsサービスのロールバック高速化
  * 社内のRuby on Railsサービス全体にCapistranoを利用した高速ロールバックを開発
  * Jenkinsサーバのメンテナンス
* Ruby on Railsサービス全体のRubyバージョンアップデート計画・実施
* EKS Cluster Blue/Greenバージョンアップデート計画・実施
  * 合わせてCircle CI/Helm/Helmfileを利用したデプロイ機構に共通化
* マイクロサービス連携基盤としてのメッセージング基盤PoC
  * Transactional Outbox Pattern/Protobuf/AWS Kinesisを採用したCDC基盤をPoC
* EC2ベースの人事労務サービスのEKS移行
  * 今後の移行プロジェクトに備え、社内共通で利用できるMulti-Role用Helmパッケージ、パラメータセットを設計・導入、既存プロジェクトも含めて標準化
* RDBMS負荷対策としてPerformance Monitoringのしくみを整備
  * MySQL sys-schema/perf-schema/info-schema/slow-log等を対象とした時系列DBをS3/AWS Athena/datadogを利用し構築・運用
* Capacity Planning
* 会計サービスDBの負荷対策
  * Reader ScalingのためAurora MySQLへの移行の移行設計・実施
  * Aurora MySQLへの移行に向け、MySQL Master-Switchover用のツールを開発・運用
  * Ruby on Rails Slow Query対策
  * 開発チームへのPerformance Review文化の浸透
  * Writer Horizontal Scaling戦略の検討評価、および実施の合意形成
* そのほかDB管理
  * MySQL/Redis/ElasticSearch/DynamoDBのインスタンスタイプ、監視、パラメータセットを標準化
  * MySQL 56からのアップデート、およびライフサイクル管理ポリシー策定
* SLOの導入
* 4-5名チームのリードエンジニアを担当
  * チームビルディング
  * OKR設定
  * 技術選定
  * 採用戦略
  * プロジェクトマネジメント

#### 人事労務サービス: SWE

2018年04月〜2019年07月

* 組織構造マスタマイクロサービスの開発・運用
  * Goによるマイクロサービス開発
  * Ruby on Railsモノリスである自社人事労務サービス給与計算モジュールとの連携機能の開発
  * モノリス間との重複管理データ同期機構の開発
  * Circle CI/CodeDeploy/Kustomizeを利用したKubernetes Clusterへのデプロイパイプライン整備
  * Kubernetes上でのサービス運用
  * Self-Host Kubernetes ClusterからEKSへのサービス移行
  * ワークフローマイクロサービスとの連携開発サポート
* Ruby on Railsによる人事労務サービス開発
  * Swaggerを用いた従業員情報Public APIの開発
  * 他社サービス間とのPublic API連携
  * Ruby on Railsモノリスである自社会計サービスとの給与連携機能の開発
  * Mackrel/newRelic/Kibanaによる監視

#### 会計サービス: Growth Engineer

2017年10月〜2018年04月

* Redshift/Redashを用いたアクティビティログの分析
* Ruby on Rails上での各種A/Bテストの設計・実施
* Ruby on Rails向けのA/B Testingモジュールの開発
* マーケティングチームがプロダクト上で施策を試しやすくできるしくみを整備


## 学歴

* 2017年9月早稲田大学政治経済学部　政治学科卒業
