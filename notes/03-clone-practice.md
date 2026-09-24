# 03 使用 git clone 获取远程仓库

## 本次目标

学习如何把 GitHub 仓库完整复制到新的本地目录。

## 完成内容

- 使用 `git clone` 克隆自己的远程仓库
- 查看克隆仓库中的文件
- 查看克隆仓库的提交历史
- 查看自动生成的 `origin` 远程配置
- 比较 `git clone` 与下载 ZIP 的区别

## 我的理解

`git clone` 不只是下载当前文件，还会下载提交历史、分支信息和远程仓库配置。

克隆完成后，新目录本身就是一个完整的 Git 仓库，并且通常已经把来源仓库设置为 `origin`。

下载 ZIP 通常只有当前文件，没有 Git 提交历史，也不能直接使用 `git pull` 获取后续更新。

## 当前成果

已经创建第二份本地仓库：

`D:\git-learning\clone-practice`

## 下一步

学习 `git fetch` 和 `git pull`，把 GitHub 上的新提交同步到本地。
