# hexo-blog

用 [hexo](https://hexo.io) 生成的博客。

访问地址：[https://ricosmall.github.io/hexo-blog/](https://ricosmall.github.io/hexo-blog/)

## 发表新文章步骤

源码都放在 source 分支，因此所有的操作都在 source 分支进行。

1. 切换到 source 分支
2. 执行 `hexo new post '文章标题'` 新建一篇文章
3. 编辑文章保存
4. 执行根目录下的脚本 `./deploy.sh` 即可发表文章到 `gh-pages` 分支

如果同时想把博客文章发表到 coding.net，按照以下步骤操作：

1. 修改根目录下的配置文件 `_config.yml`，将 `root: /hexo-blog` 改为 `/`，将 `deploy` 字段下面的 GitHub 地址注释掉，放开 Coding 地址
2. 执行根目录下的脚本 `/deploy.sh` 即可发表文章到 coding.net
3. 完成之后记得将配置文件改回原样再提交到 source 分支