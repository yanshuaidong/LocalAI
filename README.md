# LocalAI
描述



问🙋：在github上我对于别人开发的仓库，我想放在自己的仓库中，并可以拉取原开发者的更改，我自己也能向我的仓库推送文件，这要怎么做。

要实现这个功能，你可以按照以下步骤进行操作：

1. 在 GitHub 上创建一个新的仓库，作为你的仓库（假设为 A 仓库）。
2. 在本地克隆 A 仓库到你的计算机上。
3. 在 GitHub 上找到原开发者的仓库（假设为 B 仓库），并复制 B 仓库的 URL。https://github.com/go-skynet/LocalAI.git
4. 在你的计算机上使用 Git 命令行工具，使用以下命令将 B 仓库添加为 A 仓库的远程仓库：

```
git 远程的 添加 上游 https://github.com/go-skynet/LocalAI.git
git remote add upstream <B 仓库的URL>
```

这样，你就将 B 仓库添加为了 A 仓库的上游（upstream）仓库。

5. 使用以下命令拉取 B 仓库的更改：

```
git pull upstream master
```

这样，你就可以将 B 仓库的更改合并到你的本地仓库中。

6. 在本地仓库中进行你自己的修改和文件添加。

7. 使用以下命令将你的更改推送到 A 仓库：

```
git push origin master
```

这样，你就可以将你的更改推送到你的 GitHub 仓库中。

通过以上步骤，你就可以将原开发者的仓库放在你自己的仓库中，并且可以拉取原开发者的更改，同时也能向你的仓库推送文件。