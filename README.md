# ITサポート基礎演習案件パック

未経験からサーバー構築エンジニアへの就職・転職を目指す方のための、**自習用ポートフォリオ教材**です。

実際の現場で発生しそうな「案件」(依頼を受けて対応する具体的な作業)を10本用意しました。1つずつ手を動かして取り組み、作業内容と結果をGitで記録していくことで、そのまま職務経歴書やGitHubに載せられる「動くポートフォリオ」が完成する構成になっています。

全案件が「案件カテゴリ→この案件で身につくスキル→想定シナリオ→事前準備→作業目的→作業手順→完了確認チェックリスト→よくあるエラーと対処法→暗記のコツ→振り返り→ポートフォリオへの書き方例」という**同じ11セクション構成**で統一されているので、1件目を読み終えれば2件目以降は迷わず読み進められます。

> 詳しい狙いや使い方は [`docs/00_about-this-pack.md`](docs/00_about-this-pack.md) にまとめています。まずはそちらを読むのがおすすめです。

## はじめに読むもの

| ドキュメント | 内容 |
| --- | --- |
| [`docs/00_about-this-pack.md`](docs/00_about-this-pack.md) | このパックの目的・対象者・全体構成 |
| [`docs/01_roadmap.md`](docs/01_roadmap.md) | 8週間の学習ロードマップ、案件同士の前提関係 |
| [`docs/02_environment-setup.md`](docs/02_environment-setup.md) | 演習環境(VirtualBox・OSイメージ・AWSアカウント)の準備 |
| [`docs/03_beginner-start-guide.md`](docs/03_beginner-start-guide.md) | コマンドの読み方、安全確認、作業ログの残し方を学ぶ初心者向けスタートガイド |

## 案件一覧(全10案件)

| No | 案件 | カテゴリ | レベル | 目安時間 |
| --- | --- | --- | --- | --- |
| 01 | [新入社員PCキッティング対応](cases/case01_pc-setup.md) | ヘルプデスク | 初級 | 2〜3時間 |
| 02 | [社内ネットワーク疎通トラブルの切り分け対応](cases/case02_network-troubleshooting.md) | ネットワーク | 初級 | 2〜3時間 |
| 03 | [共有フォルダのアクセス権不具合対応](cases/case03_file-share-permissions.md) | Windows運用 | 初級〜中級 | 2〜3時間 |
| 04 | [Active Directoryでのユーザー・グループ管理](cases/case04_active-directory.md) | Windows Server | 中級 | 3〜4時間 |
| 05 | [Linuxサーバー初期構築](cases/case05_linux-server-setup.md) | Linux | 初級〜中級 | 3〜4時間 |
| 06 | [Webサーバー構築(Nginx)](cases/case06_web-server.md) | Linux・Web | 初級〜中級 | 2〜3時間 |
| 07 | [仮想化環境構築(VirtualBox)](cases/case07_virtualization.md) | 仮想化 | 初級 | 2〜3時間 |
| 08 | [クラウド基礎構築(AWS無料枠)](cases/case08_cloud-aws.md) | クラウド | 中級 | 2〜3時間 |
| 09 | [バックアップ・ログ監視運用](cases/case09_backup-monitoring.md) | 運用 | 中級 | 2〜3時間 |
| 10 | [セキュリティインシデント対応](cases/case10_security-incident.md) | セキュリティ | 中級 | 2〜3時間 |

ヘルプデスク的な初級案件(01〜03)から始まり、Windows/Linuxサーバー構築(04〜07)、クラウド・運用・セキュリティ(08〜10)へと段階的にステップアップする構成です。案件同士の前提関係(例: 案件04には案件07の仮想化環境が必要、案件06・09・10は案件05のサーバーが土台になる、など)は [`docs/01_roadmap.md`](docs/01_roadmap.md) で詳しく説明しています。

## 使い方の流れ

1. [`docs/02_environment-setup.md`](docs/02_environment-setup.md) を読み、演習用の環境(VirtualBoxなど)を用意する
2. [`docs/03_beginner-start-guide.md`](docs/03_beginner-start-guide.md) でコマンド例の読み方、安全な進め方、作業ログの残し方を確認する
3. [`docs/01_roadmap.md`](docs/01_roadmap.md) を読み、自分のペースで取り組む順番・スケジュールを決める
4. `cases/` フォルダの案件をロードマップの推奨順序で実施し、区切りごとにGitへコミットする
5. [`docs/91_portfolio-guide.md`](docs/91_portfolio-guide.md) を参考に、取り組んだ案件をポートフォリオとして仕上げる

## ディレクトリ構成

```text
support/
├── README.md                      ← このファイル(全体の目次)
├── cases/                         ← 10案件の詳細手順書
│   ├── case01_pc-setup.md
│   ├── case02_network-troubleshooting.md
│   ├── case03_file-share-permissions.md
│   ├── case04_active-directory.md
│   ├── case05_linux-server-setup.md
│   ├── case06_web-server.md
│   ├── case07_virtualization.md
│   ├── case08_cloud-aws.md
│   ├── case09_backup-monitoring.md
│   └── case10_security-incident.md
├── docs/                          ← 概要・ロードマップ・環境準備・用語集など
│   ├── 00_about-this-pack.md
│   ├── 01_roadmap.md
│   ├── 02_environment-setup.md
│   ├── 03_beginner-start-guide.md
│   ├── 90_glossary.md
│   └── 91_portfolio-guide.md
└── templates/
    └── case-template.md           ← 自分で案件11以降を作るときのテンプレート
```

## その他のドキュメント

- [`docs/90_glossary.md`](docs/90_glossary.md): 演習で登場するIT/インフラ基礎用語集(どの案件で登場するかも記載)
- [`docs/91_portfolio-guide.md`](docs/91_portfolio-guide.md): GitHubでの見せ方、職務経歴書への書き方例、面接対策
- [`templates/case-template.md`](templates/case-template.md): 追加の案件を自作するための空欄埋め式テンプレート

## ライセンス

このリポジトリのライセンスは [LICENSE](LICENSE) を参照してください。
