# whatoppt's Blog

个人博客源码，署名 **whatoppt**。基于 [Hexo](https://hexo.io/) + [Butterfly](https://github.com/jerryc127/hexo-theme-butterfly) 主题深度定制（青色主题配色、自定义样式、原创头图/头像/封面）。

- 线上地址：http://82.156.123.126（腾讯云轻量服务器 + Nginx 托管静态文件）
- 文章：Markdown，位于 `source/_posts/`
- 主题配置：`_config.butterfly.yml`（Butterfly 官方推荐的 data-file 方式，未直接改主题源码）
- 自定义样式：`source/css/custom.css`
- 自定义图片：`source/img/`（头像、首页头图、文章封面、favicon）

## 本地运行

```bash
npm install
npx hexo generate   # 构建到 public/
npx hexo server     # 本地预览 http://localhost:4000
```

## 发布流程

```bash
npx hexo generate
# 把 public/ 的内容同步到服务器 /var/www/blog（Nginx 根目录）
```

## 目录说明

- `source/_posts/` —— 博客文章
- `source/about/` —— 关于页
- `source/css/custom.css` —— 自定义样式
- `source/img/` —— 自定义图片资源
- `themes/butterfly/` —— Butterfly 主题（5.7.0，未修改源码，配置全在 `_config.butterfly.yml`）
- `_config.yml` —— Hexo 站点配置
