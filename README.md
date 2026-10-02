# 平精密加工 サンプルサイト

青梅信用金庫のビジネスマッチング応援サイトに掲載された企業情報をもとに作成した、提案用の非公式サンプルです。

掲載内容：金属の溶接・研磨・精密加工／所在地・電話番号

## 独自ドメイン公開の準備（2026-10-02確認）

- 対象: taira-seimitsukakou.com（取得先はXServerドメイン。取得完了は未確認）
- 現在のPages URL: https://yamaji8198.github.io/taira-seimitsu-sample/ （HTTP 200確認）
- index.htmlのメール表記・リンク: t.taira0823@gmail.com
- HTMLで参照する6画像はリポジトリに存在する。
- 現在ルートにCNAMEファイルは存在しない。

### 取得後の接続手順

1. ドメイン取得完了と綴りを確認する。
2. GitHub Settings → Pages → Custom domain に taira-seimitsukakou.com を設定する。ブランチ公開ではCNAMEファイルが作成される。
3. XServerドメインのDNSで、ドメイン直下に次のAレコード4件を設定する。

| 種別 | 対象 | 値 |
| --- | --- | --- |
| A | ドメイン直下 | 185.199.108.153 |
| A | ドメイン直下 | 185.199.109.153 |
| A | ドメイン直下 | 185.199.110.153 |
| A | ドメイン直下 | 185.199.111.153 |
| CNAME | www | yamaji8198.github.io |

4. DNSチェック完了後、HTTPSを確認し、Enforce HTTPSを有効にする。
5. 独自ドメインでトップ・画像・メールリンク・電話リンクを確認する。

DNSの反映は最大24時間、HTTPSの強制設定が利用可能になるまで最大24時間の場合がある。即時完了を保証しない。

出典（2026-10-02確認）: https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site
