# Perry 的博客

使用 [Chirpy](https://github.com/cotes2020/jekyll-theme-chirpy) 主题，通过 GitHub Actions 部署到 GitHub Pages。

站点地址：<https://yuanwei2023.github.io/perry.github.io/>

## 更新内容

- 首页自动展示 `_posts/` 中的文章，修改 `_tabs/about.md` 更新关于页面。
- 修改 `_config.yml` 设置站点标题、简介和主题。
- 在 `_posts/` 下添加 `YYYY-MM-DD-title.md` 发布文章，并在文件开头添加：

  ```yaml
  ---
  layout: post
  title: "文章标题"
  ---
  ```

提交并推送到 `main` 后，Actions 会自动构建和部署。
仓库 Settings → Pages → Build and deployment → Source 应设为 **GitHub Actions**。

## 本地预览

安装 Ruby 3.4 和 Bundler 后运行：

```sh
bundle install
bundle exec jekyll serve
```

访问 <http://localhost:4000/perry.github.io/>。
