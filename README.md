# RuntimeWarning.github.io

Personal academic homepage of Yunlong Zhou: <https://runtimewarning.github.io>

Built with [al-folio](https://github.com/alshedivat/al-folio) (v1.x) and deployed by GitHub Actions to the `gh-pages` branch.

## 日常维护

| 想改什么 | 改哪个文件 |
| --- | --- |
| 首页简介、头像旁的文字 | `_pages/about.md` |
| 头像 | 替换 `assets/img/prof_pic.jpg` |
| 论文列表 | `_bibliography/papers.bib`（`selected = {true}` 的论文会显示在首页） |
| CV 页面 | `_data/cv.yml` |
| 邮箱、Scholar、GitHub 图标 | `_data/socials.yml` |
| 期刊/会议缩写的颜色和链接 | `_data/venues.yml` |
| 网站标题、开关各种功能 | `_config.yml` |

改完推到 `main` 分支，Actions 里的 "Deploy site" 跑完（约 5 分钟）网站就会更新。

## 本地预览（可选）

需要 Ruby 3.3 + Bundler：

```bash
bundle install
bundle exec jekyll serve
```

然后打开 <http://localhost:4000>。也可以用 Docker：`docker compose up`。
