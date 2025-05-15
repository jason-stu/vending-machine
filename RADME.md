# 洪士棋

**初始化 Git**
```bash
git init
git remote add origin https://github.com/你的帳號/你的repo.git
git add .
git commit -m "Initial commit"
git push -u origin master
```


---

## 📌 1. 建立新分支

```bash
git branch 分支名稱
git checkout 分支名稱
```

### ✅ 範例：
```bash
git branch feature/login-page
```

🔎 這個指令會在你目前所在的 commit 上建立一個名為 `feature/login-page` 的新分支，但**不會自動切換過去**。

---

## 🔀 2. 切換分支

```bash
git switch 分支名稱
```

### ✅ 範例：
```bash
git checkout feature/login-page
```

🧠 如果你想要**建立並立即切換**新分支，可以用這個：
```bash
git checkout -b 分支名稱
```

### ✅ 範例：
```bash
git checkout -b feature/login-page
```

---

## 🔗 3. 合併分支

先切換到你**想要合併到的主分支**，通常是 `main` 或 `master`。

```bash
git checkout main
```

然後執行合併：

```bash
git merge 分支名稱
```

### ✅ 範例：
```bash
git merge feature/login-page
```

📌 這會把 `feature/login-page` 分支的修改內容合併到 `main` 分支中。

---

## 📋 補充：查看所有分支

```bash
git branch -a
```

## ☁️ 推送新分支到遠端

```bash
git push -u origin 分支名稱
```
# ✅ 作用解釋：

| 組件       | 解釋                                        |
|------------|---------------------------------------------|
| `git push`   | 將本地的分支推送到遠端                       |
| `切換分支`   | 建立追蹤關係（upstream），讓未來`git push`/`git`不需要再指定遠端與分支名稱                    |
| `origin` | 預設的遠端儲存庫名稱                  |
| `分支名稱`   | 要推送的本地分支名稱                         |


---

# 🧼 小提醒
- 合併前建議先使用 `git pull` 確保是最新狀態。
- 如果合併出現衝突（conflict），需手動解決後再 `git add` 和 `git commit`。

---

# ✅ 常用指令速查表

| 功能       | 指令                                        |
|------------|---------------------------------------------|
| 建立分支   | `git branch 分支名稱`                        |
| 切換分支   | `git checkout 分支名稱`                      |
| 建立＋切換 | `git checkout -b 分支名稱`                   |
| 合併分支   | `git merge 分支名稱`                         |
| 查看分支   | `git branch`                                 |
| 推送分支   | `git push -u origin 分支名稱`                |

---

