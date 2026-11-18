# D:\ 根仓库

- 位置：`D:\.git`（仓库根就是 D 盘根目录）
- 提交身份：`dong <dong@users.noreply.github.com>`
- 分支：`main`
- origin：`git@github.com:19259644091/D-root.git`（仓库名 `D-root` 为占位，可改）

## 规则

默认 `/*` 忽略顶层一切，只跟踪本文件与 `.gitignore`。这是刻意的：
整盘 265 GB，含系统目录、游戏、微信数据，既不该也不好进版本库。

要纳管某个目录，在 `.gitignore` 里加 `!目录名/` 一行，然后正常
`git add` 该目录下的具体文件。不要对整盘执行 `git add -A`。

## 改远程

```powershell
git -C "D:/" remote set-url origin git@github.com:19259644091/<仓库名>.git
```
