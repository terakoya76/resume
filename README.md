# 職務経歴書

2023年8月30日現在

Hajime Terasawa (@terakoya76)

1993年生まれ神奈川県在住

* Twitter `https://twitter.com/terakoya76`
* GitHub https://github.com/terakoya76
* Blog https://medium.com/@terako.studio
* Email `terako.studio(at)gmail.com`


## できること

* WebアプリケーションにおけるSRE/DevOps
  * アプリケーションをまたいだ問題解決とプロジェクト推進
    * 関係構築、基盤の導入支援およびセルフサービス化
  * 信頼性向上に向けた業務プロセス改善
    * SLI/SLOの設計・運用、および導入推進
    * Terraform/Ansible等のIaCによる構成管理・変更管理の導入・運用
    * CI/CD環境の構築・運用
    * Mackerel/NewRelic/Datadog等を用いた監視体制の設計・運用
    * 障害対応およびポストモーテムの設計・運用、および導入推進
  * 運用業務の自動化
    * 課題発見/設計/実装
* インフラ・ミドルウェアの構築・運用
  * ネットワークやインフラ技術の基礎的な知識
  * Docker/Kubernetesの構築・運用
  * MySQL等のRDBMSの設計・運用
  * 小規模から大規模までのAWS活用
  * 小規模のGCP活用
* バックエンド開発
  * Ruby/Go/Node.js等のプログラミング言語の経験
* その他
  * GitHubやドキュメントツール、Slack等による非同期コミュニケーション
  * 職種や技術領域をまたいだ、全体最適を目指した問題解決
  * 5人規模のチームのチームビルティング、開発計画策定、技術選定、プロジェクトマネジメント


## 職務経歴

### （株）Toreta

CTO直下の業務委託として2023年04月〜現在まで勤務（フルリモート勤務）

#### SRE (Infrastructure, Consulting)

2023年04月〜

* IaCによる変更管理の推進
  * CIの整備・設定自動化
    * Terraform/Terraform Cloud/Atlantis/GCP CloudRun/GCP CloudBuild/GCP CloudLB
  * 主要ユースケースに対するTerraformモジュール提供
* SLOによるサービス品質管理の推進
  * 開発チームとの関係構築
  * パイロットプロジェクトの選定・伴走
  * SLO定義書や振り返りなどのプラクティス啓蒙、参考実装の運用
* Observability推進
  * Datadog利用環境の整備・自動化
    * Terraform/GCP CloudRun/GCP CloudBuild/GCP CloudLB
  * Datadogのプラクティス啓蒙
* ガイドライン策定
  * IaC/SLO/Observability/Tooling
* Other
  * EKS Cluster Upgrade


### （株）obniz

CTO直下の業務委託として2021年12月〜現在まで勤務（フルリモート勤務）

#### インフラエンジニア

2021年12月〜

* セキュリティ対策
  * セキュリティ投資計画策定
  * 情報系/業務系分離の実施
  * 踏み台サーバの構築
    * STNS/google-authenticatorで実装
    * その後、STNS/Cloudflare Accessに置き換え
  * 脆弱性スキャン構築・運用
* 可用性対策
  * VPSベースのマイクロサービスアーキテクチャの耐障害性対応
    * nginxによるAPサーバ冗長化
    * pgpool2によるPostgreSQL HA構成構築
    * Cloudflare AccessによるMutli-Cloud対応
  * バックエンドサービス群の一部AWS移行設計・実施
    * Nameserver Cloudflare移行
    * 移行計画策定
    * Cloudflare WarpによるMulti-Cloud対応
    * DB単体でのAWS移行
    * AMI Build Pipeline整備
    * AP系のAWS移行
  * IaCによる変更管理の導入・運用
    * Terraform設計・運用
    * 既存Ansible Playbookの拡充・改善
  * 情報系に対するCloudflare CDN導入
  * NewRelicによる監視拡充・ガイドラインの整備・Runbook整備
* Other
  * PostgreSQLアップデート
  * 各種運用業務自動化
    * GitHub Actions Self-Hosted Runner/AWS OIDC
      * デプロイ、AMI更新
  * クラウド利用コスト最適化


### freee（株）

2017年06月〜2022年05月の間勤務（2020年よりフルリモート勤務）
* 正社員として2017年10月〜2022年05月の間勤務
* インターンとして2017年06月〜2017年09月の間勤務

#### 基盤チーム: SRE (Kitchen Sink SRE)

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
  * MySQL sys-schema/perf-schema/info-schema/slow-log等を対象とした時系列DBをS3/AWS Athena/Datadogを利用し構築・運用
* Capacity Planning
* SLOの導入
* 会計サービスDBの負荷対策
  * Reader ScalingのためAurora MySQLへの移行の移行設計・実施
  * Aurora MySQLへの移行に向け、MySQL Master-Switchover用のツールを開発・運用
  * Ruby on Rails Slow Query対策
  * 開発チームへのPerformance Review文化の浸透
  * Writer Horizontal Scaling戦略の検討評価、および実施の合意形成
* そのほかDB管理
  * MySQL/Redis/ElasticSearch/DynamoDBのインスタンスタイプ、監視、パラメータセットを標準化
  * MySQLアップデート、およびライフサイクル管理ポリシー策定
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
  * サービス間の重複管理データ同期機構の開発
  * Circle CI/AWS Codeデプロイ/Kustomizeを利用したKubernetes Clusterへのデプロイパイプライン整備
  * Kubernetes上でのサービス運用
  * Self-Host Kubernetes ClusterからEKSへのサービス移行
  * ワークフローマイクロサービスとの連携開発サポート
* Ruby on Railsによる人事労務サービス開発
  * Swaggerを用いた従業員情報Public APIの開発
  * 他社サービス間とのPublic API連携
  * Ruby on Railsモノリスである自社会計サービスとの給与連携機能の開発
  * Mackerel/NewRelic/Kibanaによる監視

#### 会計サービス: Growth Engineer

2017年10月〜2018年04月

* Redshift/Redashを用いたアクティビティログの分析
* Ruby on Rails上での各種A/Bテストの設計・実施
* Ruby on Rails向けのA/B Testingモジュールの開発
* マーケティングチームがプロダクト上で施策を試しやすくできるしくみを整備


## 学歴

* 2017年9月早稲田大学政治経済学部　政治学科卒業
