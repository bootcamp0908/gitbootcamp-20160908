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

## 13.
`git merge -ff-only`

最新リビジョンをマスターブランチとする

## 6.
`git checkout -b fix/42;git commit`
コミットを行った後、fix42のブランチを作成してHEADを作成したfix42に移動する。コミットなので変更ファイルは先にaddされている必要があるが、git commitに-aを加えればaddは省略できる。

## 14.
git merge --no-f
non-fast fowardのテスト

## 9.
`git merge`

自分のローカルリポジトリで作業したブランチをマスターにマージする。HEADはマスターのまま。

##10.
`git rebase i`

リビジョンを入れ替えたり、削除したり、統合したりすることができる。

## 16. `git remote add;git fetch`

リモートの最新状態を別ブランチでローカルに持ってくる　マージはされない

## 22. `git clone`

リポジトリにあるもの一式ローカルに落として同期された状態にする。ローカルのものは最新だけでなくリビジョンも含む

#Issue test
 #1
