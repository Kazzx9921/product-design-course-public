---
name: setup
description: 設定 GitHub 遠端 repo，讓這個專案可以 push 上去
argument-hint: （不需要額外參數，直接執行即可）
---

請幫我完成 GitHub 遠端 repo 的設定，讓我可以把這個專案推上去：

1. 詢問我的 GitHub 使用者名稱
2. 詢問我想要的 repo 名稱（預設建議：`my-lp`）
3. 提示我前往 https://github.com/new 建立一個新的**空白** public repo（不要勾選 Initialize with README）
4. 等我確認建立完成後，執行以下指令設定 remote：
   - 如果還沒有 remote：`git remote add origin https://github.com/[使用者名稱]/[repo名稱].git`
   - 如果已有 remote：`git remote set-url origin https://github.com/[使用者名稱]/[repo名稱].git`
5. 推送初始 commit：`git push -u origin main`
6. 確認推送成功，告訴我 repo 網址：`https://github.com/[使用者名稱]/[repo名稱]`

如果過程中遇到任何錯誤，請逐步引導我排除，不要略過問題。
