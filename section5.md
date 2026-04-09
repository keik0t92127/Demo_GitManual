# 🔍 5. 状態の確認

> **概要:** 作業ツリーやステージングの状態を確認します。

---

## 📋 手順

### 1. 現在の状態を確認する

```bash
git status
```

### 2. 短縮形式で確認する

```bash
git status -s
```

---

## 📊 表示の見方

| 記号 | 場所 | 意味 |
|:----:|------|------|
| `M`  | 左列（緑） | ステージ済みの変更 |
| `M`  | 右列（赤） | 未ステージの変更 |
| `A`  | 左列 | 新規追加（ステージ済み） |
| `D`  | — | 削除 |
| `??` | — | 未追跡ファイル |

### 出力例

```
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md          ← ステージ済み

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
        modified:   section1.md        ← 未ステージ

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        newfile.md                     ← 未追跡
```

---

> 💡 **ヒント:** `git status` はこまめに実行して、現在の作業状態を把握する習慣をつけましょう。  
> `git status -s` の短縮形は、変更ファイルが多い場合に便利です。

---

[← 前のセクション: コミットの作成](section4.md) ｜ [← マニュアル トップへ](gitmanual.md) ｜ [次のセクションへ → 履歴の確認](section6.md)
