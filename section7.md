# 🔎 7. 差分の確認

> **概要:** ファイルの変更内容（差分）を確認します。

---

## 📋 手順

### 1. 作業ツリーとステージの差分を表示する

```bash
git diff
```

### 2. ステージと最新コミットの差分を表示する

```bash
git diff --staged
```

### 3. 特定ファイルの差分を表示する

```bash
git diff ファイル名
```

### 4. コミット間の差分を表示する

```bash
git diff コミットID1 コミットID2
```

---

## 📊 `git diff` の対象範囲

| コマンド | 比較対象 |
|---------|---------|
| `git diff` | 作業ツリー vs ステージング |
| `git diff --staged` | ステージング vs 最新コミット |
| `git diff HEAD` | 作業ツリー vs 最新コミット |
| `git diff main feature` | main ブランチ vs feature ブランチ |

---

## 📋 出力例

```diff
diff --git a/section1.md b/section1.md
index abc123..def456 100644
--- a/section1.md
+++ b/section1.md
@@ -1,4 +1,4 @@
-# 1. Git の初期設定
+# ⚙️ 1. Git の初期設定
```

> `-` が削除された行、`+` が追加された行を示します。

---

> 💡 **ヒント:** `git diff` は未ステージの変更、`git diff --staged` はステージ済みの変更を確認できます。  
> コミット前に必ず差分を確認して、意図した変更だけが含まれているか確かめましょう。

---

[← 前のセクション: 履歴の確認](section6.md) ｜ [← マニュアル トップへ](gitmanual.md) ｜ [次のセクションへ → ブランチ操作](section8.md)
