# Git 指令教學 README

## 初始化版本庫
```bash
git init
```
初始化一個新的 Git 儲存庫。

## 設定使用者資訊
```bash
git config --global user.name "你的名字"
git config --global user.email "你的信箱"
```
設定全域使用者名稱與電子郵件。

## 檢查目前狀態
```bash
git status
```
顯示目前的版本控制狀態。

## 新增檔案到暫存區
```bash
git add 檔案名
```
加入指定檔案到暫存區。若要加入所有變更：
```bash
git add .
```

## 提交變更
```bash
git commit -m "提交訊息"
```
將暫存區的變更提交到本地版本庫。

## 檢視提交紀錄
```bash
git log
```
列出提交歷史紀錄。

## 建立新分支
```bash
git branch 分支名稱
```

## 切換分支
```bash
git checkout 分支名稱
```

## 建立並切換到新分支
```bash
git checkout -b 分支名稱
```

## 合併分支
```bash
git merge 分支名稱
```
合併指定分支到目前分支。

## 移除檔案
```bash
git rm 檔案名
```
從 Git 版本庫與工作目錄移除檔案。

## 克隆遠端儲存庫
```bash
git clone 遠端網址
```
複製遠端儲存庫到本地。

## 檢視遠端
```bash
git remote -v
```
列出設定的遠端儲存庫。

## 拉取遠端更新
```bash
git pull
```
從遠端儲存庫拉取並合併最新變更。

## 推送變更到遠端
```bash
git push
```
將本地提交推送到遠端儲存庫。

---

如需進一步進階操作，建議參考官方 Git 文件：https://git-scm.com/doc
