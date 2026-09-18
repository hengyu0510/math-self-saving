# math-self-saving

> 数院自救指南：一个基于 MkDocs Material 的数学自学指南网站。

## 网站地址

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

## 当前数学栏目

- 数学分析
- 高等代数
- 概率统计
- 实变函数
- 泛函分析
- 拓扑学
- 数值分析
- 最优化
- 数学工具

## 部署

推送 `main` 分支后，GitHub Actions 会运行：

```text
mkdocs gh-deploy --force
```

GitHub Pages 已使用 `gh-pages` 分支发布，并绑定域名 `mathselfsaving.cn`。

## TODO

- [ ] 替换站点 Logo、favicon 和标题图片
- [ ] 编写首页正式内容
- [ ] 填充各数学栏目的课程、教材、视频和习题资源
- [ ] 如需评论区，配置 Giscus 为当前仓库
- [ ] 根据需要继续调整导航结构和英文翻译
