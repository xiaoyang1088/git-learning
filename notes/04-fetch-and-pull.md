# 04 Fetch 与 Pull

## 本次目标

理解本地仓库如何获取 GitHub 上的新提交，并学会在同步前检查远程变化。

## 完成内容

- 使用第二份本地仓库模拟另一台电脑
- 使用 `git fetch origin` 获取远程最新信息
- 使用 `git log` 查看远程多出的提交
- 使用 `git diff` 比较本地与远程版本
- 使用 `git pull --ff-only` 安全同步远程更新

## 我的理解

`git fetch` 会从远程仓库获取最新提交和分支信息，但不会立即修改当前工作区。

`git pull` 会先获取远程更新，然后把更新整合到当前分支。

学习阶段可以先获取并检查变化，确认后再更新本地分支。

## Fetch 与 Pull 的区别

```text
git fetch：获取远程信息，不立即修改当前文件
git pull：获取远程信息，并更新当前分支

```

`git status` 默认不会主动连接 GitHub。它比较的是本地分支与本地已经保存的远程分支记录。

因此，在判断 GitHub 是否有新提交前，需要先执行：

```powershell
git fetch origin
```

## 推荐检查流程

```powershell
git fetch origin
git log --oneline HEAD..origin/main
git diff HEAD..origin/main
git pull --ff-only
```

这组命令依次表示：

1. 获取远程最新信息；
2. 查看远程多出的提交；
3. 查看具体文件变化；
4. 确认后安全更新本地分支。

## 下一步

学习如何使用独立分支完成任务，并通过 Pull Request 合并到 `main`。
