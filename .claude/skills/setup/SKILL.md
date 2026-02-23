---
name: setup
description: 初始化 git，建立你自己的 GitHub repo，把專案推上去
argument-hint: （不需要額外參數，直接執行即可）
---

請幫我完成以下步驟，把這個專案初始化並推上我自己的 GitHub：

1. 執行 `git init` 初始化 git 版本控制
2. 執行 `git add .` 和 `git commit -m "initial commit"` 建立第一個 commit
3. 詢問我的 GitHub 使用者名稱
4. 詢問我想要的 repo 名稱（預設建議：`my-lp`）
5. 提示我前往 https://github.com/new 建立一個新的**空白** public repo（不要勾選 Initialize with README）
6. 等我確認建立完成後，執行以下指令設定 remote 並推送：
   ```
   git remote add origin https://github.com/[使用者名稱]/[repo名稱].git
   git push -u origin main
   ```
7. 確認推送成功，告訴我 repo 網址：`https://github.com/[使用者名稱]/[repo名稱]`

如果過程中遇到任何錯誤，請逐步引導我排除，不要略過問題。
