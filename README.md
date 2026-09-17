# math-self-saving

> 一个基于 MkDocs Material 的数学自学指南网站。

<!-- TODO: 在这里补充项目简介 -->

## 网站地址

<!-- TODO: 替换成实际的 GitHub Pages 或自定义域名地址 -->

```text
https://mathselfsaving.cn/
```

## 本地开发

```powershell
python -m venv .venv
.\.venv\Scripts\python -m pip install -U pip
.\.venv\Scripts\python -m pip install -r requirements.txt
.\.venv\Scripts\python -m mkdocs serve
```

然后在浏览器打开终端输出的地址，通常是：

```text
http://127.0.0.1:8000
```

## 项目结构

```text
math-self-saving/
├── docs/              # Markdown 内容
├── overrides/         # MkDocs 主题覆盖文件
├── mkdocs.yml         # 站点配置和导航
├── requirements.txt   # Python 依赖
├── template.md        # 中文内容模板
└── template.en.md     # 英文内容模板
```

## 添加新内容

1. 在 `docs/` 下新建对应分类目录和 Markdown 文件；
2. 可参考 `template.md` 编写课程页面；
3. 在 `mkdocs.yml` 的 `nav` 中加入新页面；
4. 如果需要英文页面，同时创建对应的 `.en.md` 文件。

## 部署

推送 `main` 分支后，GitHub Actions 会运行：

```text
mkdocs gh-deploy --force
```

需要在 GitHub 仓库的 Settings → Pages 中将发布分支设置为 `gh-pages`。

## TODO

- [ ] 替换 `mkdocs.yml` 顶部的站点名称、网址和作者信息
- [ ] 删除 CS 版 `docs` 内容，建立数学学习目录
- [ ] 替换站点 Logo、favicon 和标题图片
- [ ] 配置或移除 Giscus 评论
- [ ] 完善数学课程内容和导航
