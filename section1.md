# 1. Git の初期設定

Git を使い始める前に、ユーザー名とメールアドレスを設定します。

## 手順

1. ユーザー名を設定する
   ```
   git config --global user.name "あなたの名前"
   ```
2. メールアドレスを設定する
   ```
   git config --global user.email "you@example.com"
   ```
3. 設定内容を確認する
   ```
   git config --list
   ```

> `--global` を付けると、すべてのリポジトリに共通の設定になります。リポジトリごとに変えたい場合は `--global` を省略してください。
