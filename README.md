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

- 数学基础：数学分析、高等代数、线性代数、解析几何、初等数论、离散数学
- 分析与方程：常微分方程、偏微分方程、复变函数、实变函数、泛函分析、调和分析
- 代数与几何：抽象代数、高等几何、微分几何、拓扑学、交换代数、代数数论
- 概率与统计：概率论、数理统计、随机过程、多元统计分析、时间序列分析
- 计算与应用：数值分析、计算方法、最优化、运筹学、控制论、数学建模、金融数学
- 交叉与进阶：数理逻辑、集合论、组合数学、图论、信息论、编码理论、密码学、数学物理
- 工具与写作：数学工具、数学写作、数学史

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
