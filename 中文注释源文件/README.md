# LocalAI

问🙋：在github上我对于别人开发的仓库，我想放在自己的仓库中，并可以拉取原开发者的更改，我自己也能向我的仓库推送文件，这要怎么做。

要实现这个功能，你可以按照以下步骤进行操作：

1. 在 GitHub 上创建一个新的仓库，作为你的仓库（假设为 A 仓库）。
2. 在本地克隆 A 仓库到你的计算机上。
3. 在 GitHub 上找到原开发者的仓库（假设为 B 仓库），并复制 B 仓库的 URL。https://github.com/go-skynet/LocalAI.git
4. 在你的计算机上使用 Git 命令行工具，使用以下命令将 B 仓库添加为 A 仓库的远程仓库：

```
git remote add upstream <B 仓库的URL>
```

这样，你就将 B 仓库添加为了 A 仓库的上游（upstream）仓库。

5. 使用以下命令拉取 B 仓库的更改：

```
git pull upstream master
使用允许合并无关历史的命令进行拉取。在git pull命令中添加--allow-unrelated-histories选项，如下所示：
git pull --allow-unrelated-histories upstream master
这个选项告诉Git允许合并不相关的历史记录。
```

这样，你就可以将 B 仓库的更改合并到你的本地仓库中。

6. 在本地仓库中进行你自己的修改和文件添加。

7. 使用以下命令将你的更改推送到 A 仓库：

```
git push origin master
```

这样，你就可以将你的更改推送到你的 GitHub 仓库中。

通过以上步骤，你就可以将原开发者的仓库放在你自己的仓库中，并且可以拉取原开发者的更改，同时也能向你的仓库推送文件。



<h1 align="center">
  <br>
  <img height="300" src="https://github.com/go-skynet/LocalAI/assets/2420543/0966aa2a-166e-4f99-a3e5-6c915fc997dd"> <br>
    LocalAI
<br>
</h1>

<p align="center">
<a href="https://github.com/go-skynet/LocalAI/fork" target="blank">
<img src="https://img.shields.io/github/forks/go-skynet/LocalAI?style=for-the-badge" alt="LocalAI forks"/>
</a>
<a href="https://github.com/go-skynet/LocalAI/stargazers" target="blank">
<img src="https://img.shields.io/github/stars/go-skynet/LocalAI?style=for-the-badge" alt="LocalAI stars"/>
</a>
<a href="https://github.com/go-skynet/LocalAI/pulls" target="blank">
<img src="https://img.shields.io/github/issues-pr/go-skynet/LocalAI?style=for-the-badge" alt="LocalAI pull-requests"/>
</a>
<a href='https://github.com/go-skynet/LocalAI/releases'>
<img src='https://img.shields.io/github/release/go-skynet/LocalAI?&label=Latest&style=for-the-badge'>
</a>
</p>

> :bulb: Get help - [❓FAQ](https://localai.io/faq/) [💭Discussions](https://github.com/go-skynet/LocalAI/discussions) [:speech_balloon: Discord](https://discord.gg/uJAeKSAGDy) [:book: Documentation website](https://localai.io/)
> 
> [💻 Quickstart](https://localai.io/basics/getting_started/) [📣 News](https://localai.io/basics/news/) [ 🛫 Examples ](https://github.com/go-skynet/LocalAI/tree/master/examples/) [ 🖼️ Models ](https://localai.io/models/)


[![tests](https://github.com/go-skynet/LocalAI/actions/workflows/test.yml/badge.svg)](https://github.com/go-skynet/LocalAI/actions/workflows/test.yml)[![Build and Release](https://github.com/go-skynet/LocalAI/actions/workflows/release.yaml/badge.svg)](https://github.com/go-skynet/LocalAI/actions/workflows/release.yaml)[![build container images](https://github.com/go-skynet/LocalAI/actions/workflows/image.yml/badge.svg)](https://github.com/go-skynet/LocalAI/actions/workflows/image.yml)[![Bump dependencies](https://github.com/go-skynet/LocalAI/actions/workflows/bump_deps.yaml/badge.svg)](https://github.com/go-skynet/LocalAI/actions/workflows/bump_deps.yaml)[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/localai)](https://artifacthub.io/packages/search?repo=localai)

**LocalAI** LocalAI是一个可以替代OpenAI API的REST API，可以在本地或本地部署的消费级硬件上运行LLM（以及其他模型）。它支持多个与ggml格式兼容的模型系列，而且不需要GPU。简单来说，LocalAI是一个可以在普通硬件上本地运行各种模型的软件接口。

<p align="center"><b>Follow LocalAI </b></p>

<p align="center">
<a href="https://twitter.com/LocalAI_API" target="blank">
<img src="https://img.shields.io/twitter/follow/LocalAI_API?label=Follow: LocalAI_API&style=social" alt="Follow LocalAI_API"/>
</a>
<a href="https://discord.gg/uJAeKSAGDy" target="blank">
<img src="https://dcbadge.vercel.app/api/server/uJAeKSAGDy?style=flat-square&theme=default-inverted" alt="Join LocalAI Discord Community"/>
</a>

<p align="center"><b>Connect with the Creator </b></p>

<p align="center">
<a href="https://twitter.com/mudler_it" target="blank">
<img src="https://img.shields.io/twitter/follow/mudler_it?label=Follow: mudler_it&style=social" alt="Follow mudler_it"/>
</a>
<a href='https://github.com/mudler'>
<img alt="Follow on Github" src="https://img.shields.io/badge/Follow-mudler-black?logo=github&link=https%3A%2F%2Fgithub.com%2Fmudler">
</a>
</p>

<p align="center"><b>Share LocalAI Repository</b></p>

<p align="center">

<a href="https://twitter.com/intent/tweet?text=Check%20this%20GitHub%20repository%20out.%20LocalAI%20-%20Let%27s%20you%20easily%20run%20LLM%20locally.&url=https://github.com/go-skynet/LocalAI&hashtags=LocalAI,AI" target="blank">
<img src="https://img.shields.io/twitter/follow/_LocalAI?label=Share Repo on Twitter&style=social" alt="Follow _LocalAI"/></a> 
<a href="https://t.me/share/url?text=Check%20this%20GitHub%20repository%20out.%20LocalAI%20-%20Let%27s%20you%20easily%20run%20LLM%20locally.&url=https://github.com/go-skynet/LocalAI" target="_blank"><img src="https://img.shields.io/twitter/url?label=Telegram&logo=Telegram&style=social&url=https://github.com/go-skynet/LocalAI" alt="Share on Telegram"/></a>
<a href="https://api.whatsapp.com/send?text=Check%20this%20GitHub%20repository%20out.%20LocalAI%20-%20Let%27s%20you%20easily%20run%20LLM%20locally.%20https://github.com/go-skynet/LocalAI"><img src="https://img.shields.io/twitter/url?label=whatsapp&logo=whatsapp&style=social&url=https://github.com/go-skynet/LocalAI" /></a> <a href="https://www.reddit.com/submit?url=https://github.com/go-skynet/LocalAI&title=Check%20this%20GitHub%20repository%20out.%20LocalAI%20-%20Let%27s%20you%20easily%20run%20LLM%20locally.
" target="blank">
<img src="https://img.shields.io/twitter/url?label=Reddit&logo=Reddit&style=social&url=https://github.com/go-skynet/LocalAI" alt="Share on Reddit"/>
</a> <a href="mailto:?subject=Check%20this%20GitHub%20repository%20out.%20LocalAI%20-%20Let%27s%20you%20easily%20run%20LLM%20locally.%3A%0Ahttps://github.com/go-skynet/LocalAI" target="_blank"><img src="https://img.shields.io/twitter/url?label=Gmail&logo=Gmail&style=social&url=https://github.com/go-skynet/LocalAI"/></a> <a href="https://www.buymeacoffee.com/mudler" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="23" width="100" style="border-radius:1px"></a>

</p>

<hr>

简而言之：


LocalAI是一个可以替代OpenAI API的本地REST API，它不需要GPU和互联网连接。它支持多个模型，并且在第一次加载后将模型保存在内存中，以实现更快的推理。它使用C++绑定进行推理，速度更快，性能更好。LocalAI是由Ettore Di Giacinto创建的社区驱动项目，旨在使人工智能对每个人都更加可访问。任何贡献、反馈和Pull Request都受到欢迎。请注意，这最初只是一个周末项目的有趣尝试，旨在创建像ChatGPT这样的完整AI助手所需的必要组件。社区正在迅速发展，我们正在努力使其更好、更稳定。如果您想帮助，请考虑做出贡献。

## 🔥🔥 [热门话题/路线图](https://localai.io/#-hot-topics--roadmap)

## 🚀 [功能](https://localai.io/features/)

- 📖 [使用GPT生成文本](https://localai.io/features/text-generation/) (`llama.cpp`, `gpt4all.cpp`, ... [:book: and more](https://localai.io/model-compatibility/index.html#model-compatibility-table))
- 🗣 [文本到音频](https://localai.io/features/text-to-audio/)
- 🔈 [音频到文本（使用whirlee.cpp进行音频转录）](https://localai.io/features/audio-to-text/) (Audio transcription with `whisper.cpp`)
- 🎨 [具有稳定扩散的图像生成](https://localai.io/features/image-generation)
- 🔥 [OpenAI functions](https://localai.io/features/openai-functions/) 🆕
- 🧠 [矢量数据库的嵌入生成](https://localai.io/features/embeddings/)
- ✍️ [约束语法](https://localai.io/features/constrained_grammars/)
- 🖼️ [直接从Huggingface下载模型](https://localai.io/models/)


## :book: 🎥 [媒体，博客，社交](https://localai.io/basics/news/#media-blogs-social)

- [为回应文档的团队和 OSS 项目创建一个 slackbot](https://mudler.pm/posts/smart-slackbot-for-teams/)
- [LocalAI 满 k8sgpt](https://www.youtube.com/watch?v=PKrDNuJ_dfE)
- [使用LangChain、LocalAI、Chroma和GPT4All在本地进行文档问答](https://mudler.pm/posts/localai-question-answering/)
- [将k8sgpt与LocalAI一起使用的教程](https://medium.com/@tyler_97636/k8sgpt-localai-unlock-kubernetes-superpowers-for-free-584790de9b65)

## 💻 用法

查看我们的文档中的[入门](https://localai.io/basics/getting_started/index.html) 部分。

### 💡 示例: 使用 GPT4ALL-J 模型

查看[文档](https://localai.io/basics/getting_started/#example-use-gpt4all-j-model-with-docker-compose)

### 🔗 资源

- [如何在本地建造](https://localai.io/basics/build/index.html)
- [如何在 Kubernetes 安装](https://localai.io/basics/getting_started/index.html#run-localai-in-kubernetes)
- [集成 LocalAI 的项目](https://localai.io/integrations/)

## ❤️ 赞助商