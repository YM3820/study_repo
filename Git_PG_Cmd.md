# Git コマンド

## リポジトリ作成

- git init (ローカルリポジトリ作成)

## コミットの作成

- git add (ステージングエリアに変更を登録する)
- git commit (コミットを作成する)
- git rm (Git 管理下のファイルやディレクトリを削除)

## 状態の確認

- git status 　(ローカルリポジトリの状態を確認する)
- git diff 　(各エリアの差分を確認する)
- git log 　(コミットの履歴を確認する)

## 状態の復元

- git checkout 　(ワークツリーの変更を取り消す)
- git reset（ステージングエリアに追加した変更をワークツリーへ戻す）

## リモートリポジトリ　操作

- git clone (ローカルリポジトリにコピー)
- git remote -v (リモートリポジトリ)
- git branch
- git checkout
- git push

## vscode 操作

- Ctrl + J : ターミナル表示
- Ctrl + B : サイドバー表示
- Alt + 矢印上下　でその行が
- 「エメット」
- Shift + i + TAB :

## Git コマンド

- git log --graph --oneline --all
- git reset --head
- git checkout
- git pull origin main

## ブランチ(枝訳)・マージ(合体)

- git branch newversion  
  例）git branch develop //新規 develop ブランチ作成  
  例）git branch 　//　現在ブランチ確認
- git merge newversion ※注意　 main のブランチで実行
- git log --oneline ※Git ID 確認
- git checkout XXXXXXX ※Git ID のポジションに一時的に戻れる  
  例）git checkout develop 　//　 develop 他のブランチに変更
- git branch XXXXXXX2 ※そのポジションから　新ブランチ作成
- git checkout main ※main のブランチに戻る
- git branch -D ブランチ名　※ローカルのブランチ削除
- git push origin --delete ブランチ名　※Git HUB 上のブランチを削除

## Laravel

### checkoutomposer ダウンロード

https://getcomposer.org/doc/00-intro.md#installation-windows

### composer インストール

#### composer create-project laravel/laravel SAMPLE --prefer-dist "9.\*"

### サーバー起動

#### php artisan serve

### ディレクトリ階層

#### routest/web.php

#### 中身

Route::get('/', function () {
return view('index');
});

Route::get('/welcome', function () {
return view('welcome');
});

resources/views/welcome.blade.php
