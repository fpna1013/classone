# classone
## 基本介绍

一个记录 1 班有趣的人和事的 repository  φ(゜▽゜*)♪

目前此 repository 对 public 开放

看到此处的1班成员请 star 此 repository,以便将您邀请为此 repository 的 collaborator  (^人^)

## 注意事项

原则上仅1班成员拥有此 repository 的编辑权，其他人需要修改的可以 pull requests

不同的人物志将存放不同的文件夹(例如:学生/牢璨)之中

尽可能上传格式为 .md .txt .docx或.pdf(推荐程度递减)的文本文件，图片随意（对于 markdown 不熟悉的可以搜一下教程）

一些重要通知也会写在这个文档。

## git 简易教程

对于 collaborator，首先使用在一个指定的文件夹下的 powershell cmd or bash 输入指令：

```
git clone https://github.com/fpna1013/classone/tree/main
```

在本地应该有一个 `classone` 的文件夹，使用 `cd classone` 即可进入该文件夹，也正式进入了 git。

一般来说，需要建一个分支的 branch：
```
git checkout -b your-feature-branch
```
可以任意修改上面的名字。然后开始修改。

当你任意修改完了过后，使用一下指令保存修改：

```
git add .
git commit -m 'text' 
```

其中你来修改 `text` 来简要描述你本次做的事情，例如 "change the files in 牢璨""add 温志强 biography"或者其他。

commit 过后，还在你的分支 branch 上，主 branch 和远程仓库还没有你的修改，如果你看到远程有修改。

这样的命令可以将远程仓库的修改合并到当前分支 branch：
```
git checkout main
git pull origin main
git checkout your-feature-branch
git merge main
```

如果你是直接上传到仓库，不需要在本地分支 branch 同步修改，只需要下面的命令：

```
git checkout main
git pull origin main
git merge your-feature-branch
git push origin main
```

如果出现下面的情况，请检查你的网络连接：
```
fatal: unable to access 'https://github.com/fpna1013/classone/': Failed to connect to github.com port 443 after 21057 ms: Timed out
```

否则的话你就可以看到正常的上传，远程仓库就有你的文件了！

## 一些问题

如果在你修改 main branch 的时候又有其他的上传，使用以下的步骤：
```
git stash
git pull
git stash pop
git commit -m 'text'
git push origin main
```
注意修改 `text` 中的内容。

如果你需要了 conflict，请找到 conflict 的文件做出修改（在这个文件内会有两个冲突的版本），然后：

```
git add x.x
```

然后正常的 `commit, push` 即可。

## 最后

向所有为此 repository 以及其他1班建设作出贡献者致敬  (^^ゞ\