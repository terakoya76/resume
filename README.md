# 職務経歴書

2024年03月06日現在

Hajime Terasawa (@terakoya76)

1993年生まれ神奈川県在住

* Twitter `https://twitter.com/terakoya76`
* Bluesky `https://bsky.app/profile/terakoya76.bsky.social`
* GitHub https://github.com/terakoya76
* Blog https://medium.com/@terako.studio
* Email `terako.studio(at)gmail.com`


## できること

* WebアプリケーションにおけるSRE/DevOps
  * アプリケーションをまたいだ問題解決とプロジェクト推進
    * 問題提起・ソリューション開発
    * 各チームとの関係構築
    * 基盤の導入支援およびセルフサービス化
  * 信頼性向上に向けたアーキテクチャ/業務プロセス改善
    * インフラ設計・改善
    * SLI/SLOの設計・運用、および導入推進
    * Terraform/Ansible等のIaCによる構成管理・変更管理の導入・運用
    * CI/CD環境の構築・運用
    * Mackerel/NewRelic/Datadog等を用いた監視体制の設計・運用
    * 障害対応およびポストモーテムの設計・運用、および導入推進
    * ガイドライン整備
  * 運用業務の自動化
    * 課題発見/設計/実装
* インフラ・ミドルウェアの構築・運用
  * ネットワークやインフラ技術の基礎的な知識
  * Docker/Kubernetesの構築・運用
  * MySQL等のRDBMSの設計・運用
  * 小規模から大規模までのAWS活用
  * 小規模のGCP活用
  * VPS/PaaSを利用した安価なサービス提供
* バックエンド開発
  * 要件定義
  * Ruby/Go/Node.js等のプログラミング言語の経験
* その他
  * GitHubやドキュメントツール、Slack等による非同期コミュニケーション
  * 職種や技術領域をまたいだ、全体最適を目指した問題解決
  * チームビルティング、開発計画策定、技術選定、プロジェクトマネジメント


## 職務経歴

### 世界史Database

業務委託として2023年12月から現在まで勤務（フルリモート勤務）

データ品質を向上させる枠組みづくりがミッション

#### SWE

2023年12月〜

* IaCによる変更管理の推進
  * やったこと
    * CIの整備・設定自動化
  * 利用技術
    * Terraform/Digger
* データ分析基盤の設計・構築
  * やったこと
    * DBの日時スナップショットを、Data Lakeを経由してDWHに連携するしくみの構築
  * 利用技術
    * Terraform
    * AWS RDS(Golden Source)/AWS S3(Lake)/Snowflake(DWH)/ETL(AWS ECS/dbt)
* Other
  * RDS証明書更新


### 医療DX

受託制作

ユーザーテストに向けた医療DXサービスのプロトタイプ制作

#### SWE

2023年12月〜2024年2月

* ユーザーテストに向けた医療DXサービスのプロトタイプ制作
  * やったこと
    * やりたいことをヒアリングし、そこから要件定義
    * 機能・コストを最小化した設計・実装
  * 利用技術
    * Swift/SwiftUI/HealthKit/Firebase Authentication/Firebase Storage/GAS


### 飲食業界向けB2B SaaS

CTO直下の業務委託として2023年04月〜現在まで勤務（フルリモート勤務）

各マイクロサービス開発チームが `You build it, you run it` を実践できるよう、しくみを整備することがミッション

#### SRE (Infrastructure, Consulting)

2023年04月〜

* IaCによる変更管理の推進
  * やったこと
    * CIの整備・設定自動化
    * 主要ユースケースに対するTerraformモジュール提供
    * ガイドライン整備
  * 利用技術
    * IaC: Terraform/Terraform Cloud/Atlantis
    * Infra: GCP CloudRun/CloudBuild/CloudLB
* SLOによるサービス品質管理の推進
  * やったこと
    * 参考実装として社内サービスのSLO運用
    * 開発チームとの関係構築
    * パイロットプロジェクトの開始・伴走
    * SLO定義書や振り返りなどのプラクティス啓蒙
    * 設定状況のチェック/レポート
  * 利用技術
    * SaaS: Datadog
* Observability推進
  * やったこと
    * Datadog利用環境の整備・自動化
    * SaaS系ガイドライン整備
    * ワークショップ実施によるDatadogのプラクティス啓蒙
  * 利用技術
    * Infra: GCP CloudRun/CloudBuild/CloudLB
    * Auth: Auth0/GCP Workload Identity/OIDC Federation
* Other
  * AWS EKS Cluster Upgrade
  * メール認証周り（SPF/DKIM/DMARC）
  * Legacy Monolithの考古学・ドキュメント作成・保守作業
  * 情シスチームへのアカウント管理業務の移管
  * Cloudコスト最適化


### IoT Platform

CTO直下の業務委託として2021年12月〜2023年10月の間勤務（フルリモート勤務）

1人目インフラエンジニアとして、インフラ周りを整理するのがミッション

#### インフラエンジニア

2021年12月〜2023年10月

* セキュリティ対策
  * セキュリティ投資計画策定
  * セキュリティ対策
    * やったこと
      * 情報系/業務系分離の計画・実施
      * 踏み台サーバの構築
      * 脆弱性スキャン構築・運用
    * 利用技術
      * VPS
      * STNS/google-authenticator/vuls
      * Cloudflare CDN/Cloudflare Access
      * AWS ASG/ELB
      * Ansible/Terraform
* 可用性対策
  * VPSベースのマイクロサービスアーキテクチャの耐障害性対応
    * やったこと
      * APサーバ冗長化
      * PostgreSQL HA化
      * Mutli-Cloud対応
    * 利用技術
      * VPS
      * nginx/PostgreSQL/pgpool2
      * Cloudflare Access
      * Ansible/Terraform/GitHub Actions
  * バックエンドサービス群の一部AWS移行の計画・実施
    * やったこと
      * 移行計画策定
      * Nameserver移行
      * 移行過渡期におけるMulti-Cloud対応
      * DBのAWS移行
      * AP系のAWS移行
      * CI/CD整備・自動化
    * 利用技術
      * Cloudflare/Cloudflare Warp
      * AWS RDS(PostgreSQL)/ELB/ASG/EC2 Image Builder
      * Ansible/Terraform/GitHub Actions
* 運用の体系化
  * やったこと
    * ガイドラインの整備
    * 監視ルール拡充・Runbook整備
    * IaCによる変更管理の導入・運用
    * CI/CD整備
    * スケールアウトプロセスの標準化・省力化
  * 利用技術
    * VPS
    * NewRelic
    * Ansible/Terraform/GitHub Actions
* Other
  * PostgreSQLアップデート
  * クラウド利用コスト最適化、およびプロセスの自動化
  * メール認証周り（SPF/DKIM）
  * 障害対応


### freee（株）

2017年06月〜2022年05月の間勤務（2020年よりフルリモート勤務）
* 正社員として2017年10月〜2022年05月の間勤務
* インターンとして2017年06月〜2017年09月の間勤務

#### 基盤チーム: SRE (Kitchen Sink SRE)

2019年08月〜2022年05月

* Ruby on Railsサービス群の保守運用
  * やったこと
    * EC2ベースのRuby on Railsサービス群に向け、Capistranoを利用した高速ロールバック機能を開発・導入
    * Jenkinsメンテナンス
    * EC2ベースのRuby on Railsサービス群のRubyバージョンアップデート計画・実施
    * EC2ベースのRuby on RailsモノリスのEKS移行
    * EKS移行効率化のための、Helmテンプレート、パラメータセットを設計・導入し、既存プロジェクトも含めて標準化した
    * Capacity Planning
    * 障害対応
  * 利用技術
    * Ruby on Rails
    * AWS ASG/ELB/RDS(MySQL)/Elasticache(Redis)/OpenSearch/SQS/Lambda/EKS
    * Jenkins/Capistrano/Packer/Vagrant/Ansible/Terraform/Helm/Helmfile/Circle CI
    * NewRelic/Mackerel/Datadog
* EKS Clusterの保守運用
  * やったこと
    * Capacity Planning
    * Blue/Greenバージョンアップデート計画・実施
    * CI/CDを単純化するため式年遷宮
  * 利用技術
    * AWS EKS/ELB/RDS
    * Helm/Helmfile/Circle CI
* マイクロサービス連携基盤としてのメッセージング基盤
  * やったこと
    * Transactional Outbox Pattern/Protobuf/AWS Kinesisを採用したCDC基盤をPoC
  * 利用技術
    * Ruby on Rails/Protobuf/MySQL
    * AWS KinesisDataStream/SQS/ElasticSearch/
* DBの運用保守
  * やったこと
    * Performance Monitoringのための時系列DB構築・運用
    * 負荷対策
      * Reader ScalingのためAurora MySQLへの移行の計画・実施
      * Aurora MySQLへの移行に向け、MySQL Master-Switchover用のツールを開発・運用
      * Slow Query対策
      * Writer Horizontal Scaling戦略の検討評価、および実施の合意形成
    * サービスへのSLOの導入
    * 開発チームへのPerformance Review文化の浸透
    * MySQL/Redis/ElasticSearch/DynamoDBのインスタンスタイプ、監視ルール、パラメータセットを標準化
    * 各サービスのMySQLバージョンのアップデート
    * MySQLバージョンのライフサイクル管理ポリシー策定
  * 利用技術
    * Ruby on Rails/Go
    * MySQL sys-schema/perf-schema/info-schema/slow-log
    * AWS S3/Athena/RDS/Elasticache/OpenSearch/DynamoDB
    * Datadog
* 4-5名チームのリードエンジニアを担当
  * チームビルディング
  * OKR設定
  * 技術選定
  * 採用戦略
  * プロジェクトマネジメント

#### 人事労務サービス: SWE

2018年04月〜2019年07月

* 組織構造マスタマイクロサービスの開発・運用
  * やったこと
    * Goによるマイクロサービス開発
    * モノリスである人事労務サービスの給与計算モジュールとの連携機能の開発
    * サービス間の重複管理データ同期機構の開発
    * CI/CD整備
    * Kubernetes上でのサービス運用
    * Self-Host Kubernetes ClusterからEKSへのサービス移行計画・実施
    * ワークフローマイクロサービスとの連携開発サポート
  * 利用技術
    * Go/Ruby on Rails/React.js/Storybook
    * nginx
    * AWS EKS/RDS(MySQL)/Elasticache(Redis)/ELB
    * Circle CI/AWS CodeDeploy/Kustomize
* Ruby on Railsによる人事労務サービス開発
  * やったこと
    * 従業員情報Public APIの開発
    * 他社サービス間とのPublic API連携
    * モノリスである自社会計サービスとの給与連携機能の開発
    * 監視ルールの整備・運用
  * 利用技術
    * OAuth
    * Ruby on Rails/Swagger
    * nginx
    * Mackerel/NewRelic/Kibana/ElasticSearch

#### 会計サービス: Growth Engineer

2017年10月〜2018年04月

* Ruby on Rails上での各種A/Bテストの設計・実施
  * やったこと
    * アクティビティログの分析
    * テスト計画・実装・評価
  * 利用技術
    * Ruby on Rails/CSS/JavaScript
    * Redshift/Redash
* Ruby on Rails向けのA/B Testingモジュールの開発
  * やったこと
    * 動的なテスト開始終了設定・重み付け管理などの機能を提供するRails Engine Gem開発
  * 利用技術
    * Ruby on Rails
    * MySQL/Redis
* マーケティングチームがプロダクト上で施策を試しやすくできるしくみを整備
  * やったこと
    * マーケティングチームが独立してアフィリエイト配信できるようしくみを開発
  * 利用技術
    * JavaScript
    * Google Tag Manager


## 学歴

* 2017年9月早稲田大学政治経済学部　政治学科卒業
