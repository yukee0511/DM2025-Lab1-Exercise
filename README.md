# DM2025-Lab1

ISA5810 Lab 1
# git 操作方法
## 檢視以往log 
```terminal
git log --oneline -n
// -n 是察看筆數，視需要改變
// e.g. git log --oneline -3
// 查看前三筆資料
```
## 回復到某版本
```terminal
git reset vesion_id
// vesion_id 是透過log查詢出來的
// e.g.
// git log --oneline -3
// 783c892 (HEAD -> main, origin/main, origin/HEAD) 練習一完成
// 00c5ffd 增加啟動文件
// c84a8f4 (upstream/main, upstream/HEAD) add explanation of change code of PAMI
// git reset 00c5ffd // 恢復至"增加啟動文件版本"

```
## 推送新版本至github
```terminal
git add . // 新增所有文件到本地快取
git commit -m '提交的訊息' // 提交訊息請自行修改為當前狀態
git push origin main
```