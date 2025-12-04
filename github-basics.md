# GitHubの基本操作

## GitHubとは

GitHubは、GitリポジトリをホスティングするWebサービスです。コードの共有、コラボレーション、バージョン管理を簡単に行えます。

## 基本的な操作

### リモートリポジトリの追加

```bash
git remote add origin <リポジトリのURL>
```

GitHubで作成したリポジトリをローカルのリモートとして追加します。

### リモートリポジトリの確認

```bash
git remote -v
```

設定されているリモートリポジトリを確認します。

### プッシュ（アップロード）

```bash
git push -u origin main
```

ローカルの変更をGitHubにアップロードします。`-u`オプションで上流ブランチを設定します。

### プル（ダウンロード）

```bash
git pull origin main
```

GitHubの変更をローカルにダウンロードします。

### クローン

```bash
git clone <リポジトリのURL>
```

既存のリポジトリをローカルにコピーします。

## GitHubでの作業フロー

### 1. リポジトリの作成

1. GitHubにログイン
2. 右上の「+」ボタンから「New repository」を選択
3. リポジトリ名を入力して作成

### 2. ローカルとリモートの接続

```bash
git remote add origin https://github.com/ユーザー名/リポジトリ名.git
git branch -M main
git push -u origin main
```

### 3. 変更のプッシュ

```bash
git add .
git commit -m "変更内容の説明"
git push
```

## プルリクエスト（Pull Request）

1. 新しいブランチで変更を加える
2. そのブランチをGitHubにプッシュ
3. GitHub上で「Pull Request」を作成
4. レビューを受けてマージ

## 練習問題

1. GitHubで新しいリポジトリを作成してみましょう
2. このプロジェクトをGitHubにプッシュしてみましょう
3. 新しいブランチで変更を加えて、プルリクエストを作成してみましょう

