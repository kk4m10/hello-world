# git-tutorial

## 主なgitコマンド
- commit

    ファイルの変更をリモートレポジトリに記録する。
    その際にいつだれがどのような変更をしたかをメッセージに残す。
- add

    コミットしたいファイルを登録する。
- push

    commitされた変更をリモートレポジトリに反映させる。
- pull

    リモートレポジトリの内容をローカルレポジトリに反映させる
- request-pull

    ローカルレポジトリの変更依頼を出す
- branch

    mainとは異なるルートを作成する。ここでの変更は操作しない限りmainのブランチに干渉しない。

- clone

    レポジトリをコピーする
- checkout

    今いるbranchから別のbranchへと切り替える。


# 一般的なGitフロー

## リポジトリの作成またはクローン
- git init（新規作成）
- git clone <repository URL>（既存のリポジトリをクローン）

## ブランチの作成
- git branch <branch>

## ブランチの切り替え
- git checkout <branch>

## コードの変更とコミット
- ファイルを編集し、git add <file>でステージングし、git commit -m 
"commit message"でコミットする

## リモートリポジトリへのプッシュ
- git push -u origin <branch>

## プルリクエストまたはマージリクエストの作成
- コードの変更を他の開発者に通知し、コードのレビューやマージを行う

## レビューと修正
- コードの変更に対するフィードバックを受け、必要な修正を行う

## マージ
- コードが承認されたら、マージを実行して変更を本番環境に統合する

## - メインブランチへのマージ
- 開発が安定し、テストが完了した場合は、メインブランチにマージする