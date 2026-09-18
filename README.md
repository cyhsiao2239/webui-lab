# WebUI Lab

Web Programming課程實作專案。


## 學號
114213519

## 本機執行
```bash
npm install
npm run dev
```

## 延伸練習
git add . 跟 git add -A 有什麼差別？
`git add .` 和 `git add -A` 都是把檔案放入「下一次 commit 的暫存區」，主要差別在範圍：

| 指令 | 作用範圍 |
|---|---|
| `git add .` | 目前資料夾及其子資料夾 |
| `git add -A` | 整個 Git 專案，包含所有新增、修改、刪除的檔案 |

例如目前位於專案根目錄：

```powershell
git add .
```

通常和：

```powershell
git add -A
```

效果相同。

但如果進入子資料夾後執行：

```powershell
cd src
git add .
```

只會加入 `src` 底下的變更；而：

```powershell
git add -A
```

會加入整個專案的變更。

若想一次加入整個專案，建議使用：

```powershell
git add -A
git commit -m "描述這次修改"
```

補充：`git add -u` 只會加入已追蹤檔案的修改與刪除，不會加入新檔案。