# 语桥官网

参照 dolog-site 的 Jekyll 结构与视觉风格构建，部署目标为 GitHub Pages，域名为 https://lingox.cn。

## 本地预览

```sh
bundle install
bundle exec jekyll serve
```

## 部署与域名

在 GitHub 仓库 Settings → Pages 中选择 Deploy from a branch，使用 `main` 分支的根目录，并将 Custom domain 设置为 `lingox.cn`。仓库的 `CNAME` 与 `_config.yml` 已配置该域名。

在域名服务商添加以下记录：

| 类型 | 主机记录 | 值 |
| --- | --- | --- |
| A | @ | 185.199.108.153 |
| A | @ | 185.199.109.153 |
| A | @ | 185.199.110.153 |
| A | @ | 185.199.111.153 |
| CNAME | www | habitism.github.io |

DNS 验证和证书签发完成后，在 Pages 设置中启用 Enforce HTTPS。详情见 [GitHub 官方文档](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site/managing-a-custom-domain-for-your-github-pages-site)。

## 应用链接

App Store： https://apps.apple.com/app/id6708231214

应用隐私政策和使用条款使用 `/privacy/`、`/eula/`，保持原链接兼容。
