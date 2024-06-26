---
layout:     post
title:      "Hello World"
subtitle:   " \"你好世界！你好博客！\""
date:       2024-05-13 13:44:00
author:     "Li Junhao"
header-img: "img/post-bg-2015.jpg"
catalog: true
tags:
    - Meta
---


## 关于我

你好啊！我是李均灏。这里是我的个人博客，用于分享自己平时折腾电脑，程序以及大佬开源项目的过程。


## 关于博客

这套博客基于[Hux Blog](https://github.com/Huxpro/huxpro.github.io)修改而来，感谢Hux的**开源**!
### 开源？什么是开源呢？
*在我的博客中，我会提到很多关于开源的概念，希望能帮助你了解一下。*

开源一词最初是指开源软件（OSS）。**开源软件是源代码可以任意获取的计算机软件，任何人都能查看、修改和分发他们认为合适的代码。**

开源软件**依托同行评审和社区生产**，皆以分散、协作的方式开发。**开源软件由社区开发，而非单个作者或公司，因此通常成本更低、更灵活，寿命比专有软件更长**。

开源已成为一种超越软件生产界限的运动和工作方式。**开源运动旨在利用开源软件的价值和分散的生产模型，为其社区和行业的问题寻找新的解决方法**。

开源软件的价值主要体现在以下几个方面：

- **同行评审**：由于源代码可自由访问，而且开源社区非常活跃，因此同行程序员会积极检查和改进开源代码。它就如同充满活力和生机的代码，而不是固步自封、停滞不前。
- **透明性**：想要准确了解哪些类型的数据移动到哪里，或代码中发生了哪些类型的变化？开源允许您自行检查和跟踪，不必依赖供应商承诺。
- **可靠性**：专有代码只靠单个作者或控制该代码的公司来更新、修复和保持正常工作。开源代码的存在时间可以超越其原作者，因为活跃的开源社区会不断进行更新。开放标准和同行评审可以确保开源代码经常得到适当的测试。
- **灵活性**：由于开源代码注重修改，因此您可以使用它来解决您的业务或社区面临的独特问题。您不再只能用一种特定方式使用代码，您可以依托社区帮助和同行评审帮助您实施新解决方案。
- **更低成本**：因为开源，所以代码本身是免费的，当您使用红帽等公司时，您只用为支持、安全强化和管理互操作性帮助等服务买单。
- **无供应商锁定**：赋予用户自由，意味着您可以随时随地使用开源代码，用于任何目的。
- **开放式协作**：活跃的开源社区，让您不再囿于方寸天地，而是能获得超越兴趣小组或者一个公司的帮助、资源和观点。

**摘自[Red Hat社区](https://www.redhat.com/zh/topics/open-source/what-is-open-source)**

## 正文
接下来说说搭建这个博客的技术细节。  

正好之前就有关注过 [GitHub Pages](https://pages.github.com/) + [Jekyll](http://jekyllrb.com/) 快速 Building Blog 的技术方案，非常轻松时尚。[~~早期李均灏的个人网站~~](htpps://mcmcljx.github.io/mcmcljx)

其优点非常明显：

* **Markdown** 带来的优雅写作体验
* 非常熟悉的 Git workflow ，**Git Commit 即 Blog Post**
* 利用 GitHub Pages 的域名和免费无限空间，不用自己折腾主机
* 如果需要自定义域名，也只需要简单改改 DNS 加个 CNAME 就好了 
* Jekyll 的自定制非常容易，基本就是个模版引擎

配置的过程中也没遇到什么坑，基本就是 Git 的流程，相当顺手

---
如何开始搭建自己的博客呢？

1. 首先，你需要一个 [GitHub](https://github.com/) 账号，因为博客基于 Git 来管理，需要有一个远程仓库。

![img](/img/screenshot-1715578881958.png)

2. 然后，fork [Huxpro/huxpro.github.io](https://github.com/Huxpro/huxpro.github.io) 项目，Fork 是指复制一份仓库，但是与原仓库不同，你拥有自己的一份仓库，可以任意修改。(点击右上角的 Fork 按钮,)

![img2](/img/screenshot-1715579411989.png)

3. 接着，修改仓库名为 `username.github.io`，其中 `username` 是你的 GitHub 用户名。
![img3](/img/IMG_20240513_140210.jpg)

4. 选择你刚才 Fork 的仓库，然后点击 Settings 按钮。

![img4](/img/screenshot-1715580482438.png)

5. 找到pages部分，会发现一个“Build and deployment”的选项，点击Github action。

![img5](/img/screenshot-1715661267421.png)

6. 下面会提示我们可以选择一个工作流，这里我们选择jekyll。

![img6](/img/IMG_20240514_124610.jpg)
7. 点击Start commit，然后点击Commit new file。
![img7](/img/IMG_20240514_124630.jpg)

![img7](/img/Screenshot_2024-05-14-12-48-10-559-edit_com.ss.android.ugc.aweme.jpg)

8. 打开Actions页面.

![img8](/img/Screenshot_2024-05-14-12-49-21-130-edit_com.ss.android.ugc.aweme.jpg)

9. 可以看到，Actions已经开始运行了。

![img9](/img/Screenshot_2024-05-14-12-58-56-231_com.ss.android.ugc.aweme.jpg)

10. 等Actions运行完毕，就可以通过 `http://username.github.io` 访问你的博客啦！**(username 是你的 GitHub 用户名)**

![img10](/img/Screenshot_2024-05-14-12-59-18-172_com.ss.android.ugc.aweme.jpg)

11. 最后，修改 `_config.yml` 文件，把 `title`、`name`、`email`、`description` 等信息改成你自己的，然后就可以开始写博客啦！

12. 当然，你也可以直接修改 `README.md` 文件来写博客，不过这样就没有目录结构，不利于管理。

13. 如果你想绑定自己的域名，可以去购买一个域名，然后在你的 DNS 解析设置中，将域名的DNS 记录改成 `username.github.io` 解析到 GitHub Pages 的 IP 地址。

这样，你就可以通过 `http://username.github.io` 访问你的博客啦！**(username 是你的 GitHub 用户名)**

---

**最后，感谢阅读，希望你能喜欢这个博客。**
