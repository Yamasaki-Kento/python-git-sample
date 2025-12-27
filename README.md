# python-git-sample

## 1. 仮想環境の準備

### ① Python が使えるか確認

```bash
py --version
```

### ② 仮想環境を作成（標準 venv）

プロジェクト直下で実行：

```bash
py -m venv .venv
```

### ③ 仮想環境を有効化（Git Bash 用）

⚠ **PowerShell / cmd とコマンドが違うので注意**

```bash
source .venv/Scripts/activate
```

### ④ pip のアップデート（初回推奨）

```bash
py -m pip install --upgrade pip
```

## 2. 依存関係をインストール

### ①numpyをインストール

```bash
pip install numpy==2.3.5
```

### ②依存関係のアウトプット

```bash
pip freeze > requirements.txt
```

### ③依存関係をインストール

```bash
pip install -r requirements.txt
```

## 3. プルリクエストを出す

## 4. マージ

## 5. feature/upgrade-numpy ブランチを作成

```bash
git checkout -b feature/upgrade-numpy
```

## 6. numpyのバージョンアップ

```bash
pip install --upgrade numpy
```

## 7. アプリの実行

### 成功したらプルリクエスト＆マージする

成功したら、requirements.txt を更新してプルリクエストを出し、マージします。

```bash
pip freeze > requirements.txt
```

### 失敗したらmainブランチに戻って元のバージョンに戻す

```bash
git checkout main
pip install -r requirements.txt
```
