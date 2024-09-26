## 個人ブログ　

アンチエイジングなど、自分の興味を持った研究や読書の内容を紹介しています。

### 作成した技術スタック

使用言語:Go
フレームワーク:
- Hugo
  - テーマ:marmaid

CI/CD: GithubActions

デプロイ: GithubPages

公開URL: https://mametaro99.github.io

## 作ろうと思った動機


2024年まで、有料であるレンタルサーバ、ドメインやWordPressを使って、ブログサイトを運営していました。
そこで、自分でブログサイトを開発して、料金のかからないGithubActionsを使用することで、
本来かかるレンタルサーバやドメインなどの費用を節約しようと考えました。

## この開発で学んだこと

### Hugoについて

goで作られていたWebフレームワークで、
数回のコマンドや、ファイルの設定をすることで、静的なWebサイトが生成されて、起動することができます。
コーディングしなくてもWebサイトを起動することができるため、プログラミングが苦手な人にもおすすめです。

## 工夫したこと

GithubActionsを使って、push時にActionsに自動デプロイできるようにしたことです。
自動的にデプロイできるようにすることで、記事の作成・編集を行いPushを行ったときに、
自動で公開されるWebページが更新されるようになります。これによって、
本来必要なコードの変更のたびにデプロイのためのコマンドを打つ必要が無くなすことができました。

## とくに、苦労したこと

公開されているHugo用のGithubActionsのドキュメントでは、
指定されているOSやHugoのバージョンが異なっており、
エラーがでてしまい、本番環境にBuildすることができませんでした。
エラーをWeb検索して、問題の箇所を特定してバージョンの変更を行うことで、Buildを行うことができました。
