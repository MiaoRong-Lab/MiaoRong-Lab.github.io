# 荣淼课题组主页

这是上海大学机电工程与自动化学院荣淼课题组的 GitHub Pages 主页源码，基于 [al-folio](https://github.com/alshedivat/al-folio) 和 Jekyll 构建。

线上访问地址：

https://miaorong-lab.github.io/

## 本地预览

推荐使用 Docker 预览，避免本机 Ruby/Jekyll 环境配置问题。

```powershell
docker compose pull
docker compose up -d
```

启动后访问：

http://localhost:8080/

如果修改了 `_config.yml`，需要重启容器：

```powershell
docker compose down
docker compose up -d
```

## 常用维护位置

- 首页内容：`_pages/about.md`
- 论文列表：`_bibliography/papers.bib`
- 新闻动态：`_news/`
- 图片资源：`assets/img/`
- 全站配置：`_config.yml`
- 样式调整：`_sass/`

## 部署说明

源码维护在 `main` 分支。推送到 `main` 后，GitHub Actions 会自动构建静态页面，并发布到 `gh-pages` 分支。

GitHub Pages 设置中保持：

- Source: `Deploy from a branch`
- Branch: `gh-pages`
- Folder: `/root`
