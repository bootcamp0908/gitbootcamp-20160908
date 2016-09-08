# 自己紹介

- bootcamp0908

  中森と申します。よろしくお願いします。

- account

# git のコマンド解説

## 3.
`git commit -a`
addとcommitを一括で行う。
結果はgit add を行ってから、git commitを行った場合と同じ。
ただし、ファイル指定をしないため意図しない変更がコミットまで進んでしまう可能性がある。

## 4.
`git commit --amend`

直前のコミットを全く別のコミットで置き換える

## 5. `git branch fix/42`

自分のローカルリポジトリに "fix/42" というブランチを作る。作るだけ。HEAD は移動しない。

## 6.
`git checkout -b fix/42;git commit`
コミットを行った後、fix42のブランチを作成してHEADを作成したfix42に移動する。コミットなので変更ファイルは先にaddされている必要があるが、git commitに-aを加えればaddは省略できる。

## 9. `git merge`

差分をマージする。master以外のブランチの差分をmasterに反映する。

## 10. `git rebase i`

リビジョンを入れ替えたり、削除したり、統合したりすることができる。

## 12.
`git checkout`

ブランチのHEADを移動する。それ以上の操作はなく、指定したブランチを作るわけでもない。そのため存在しないブランチを指定した場合にはエラーとなる。

## 13. `git merge -ff-only`

最新リビジョンをマスターブランチとする

## 14.
git merge --no-f
non-fast fowardのテスト

## 15.	 `git fetch`

リモートリポジトリの最新の情報をローカルに持ってくる。持ってくるだけで、自分の編集内容が上書きされたりするわけではないよ。

## 16. `git remote add;git fetch`

リモートの最新状態を別ブランチでローカルに持ってくる　マージはされない
git remote add => リモートリポジトリを追加
git fetch =>pullを実行すると、リモートリポジトリの内容のマージが自動的に行われてしまいます。しかし、単にリモートリポジトリの内容を確認したいだけの時はマージをしたくない場合もあります。そのような時はfetchを使用します。
メモ 17 'git pull'
pullを実行するとリモートリポジトリの履歴を取得することができます。
メモ18 'git pull -rebase'


## 18. `git pull --rebase`

リモートの最新を fetch して、そこに自分の修正を rebase で取り込む。マージコミットが作られないので、履歴が直線的になる。

## 19. `git push`

ローカルのリポジトリのリビジョンをリモートリポジトリに追加する。origin/masterがHEADと一致する。

## 21. `git init`

git リポジトリを作成するコマンド。既存のファイル群を git のリポジトリにすることも、空の新規リポジトリを作成することも可能。.git ディレクトリが生成される。

## 22. `git clone`

大抵のgitプロジェクトでは、githubなどから自分の環境にクローンを作成するところからはじまる。基本文法は以下の通り. $ git clone <uri>. このuriの中に入るのは、http,httpsから始まるurlやsshプロトコルで指定するもの.


# Issue test
 #1
