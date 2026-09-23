\# 04 Fetch 与 Pull



\## 本次目标



理解本地仓库如何获取 GitHub 上的新提交。



\## 完成内容



\- 使用第二份本地仓库模拟另一台电脑

\- 使用 `git fetch origin` 获取远程最新信息

\- 使用 `git log` 查看远程多出的提交

\- 使用 `git diff` 比较本地与远程版本

\- 使用 `git pull --ff-only` 安全同步远程更新



\## 我的理解



`git fetch` 会从远程仓库获取最新提交和分支信息，但不会立即修改当前工作区。



`git pull` 会先获取远程更新，然后把更新整合到当前分支。



学习阶段可以先使用 `git fetch` 检查远程变化，确认后再使用 `git pull --ff-only`。



\## Fetch 与 Pull 的区别



```text

git fetch：获取远程信息，不立即修改当前文件

git pull：获取远程信息，并更新当前分支

