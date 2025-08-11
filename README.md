# tsinghua_birdisland.github.io

这是清华大学"鸟岛与少年"实践支队的官方网站，展示支队历年来的生态保护成果和实践活动。

## 网站结构

```
tsinghua_birdisland.github.io/
├── index.html                  # 网站首页（已存在）
├── _config.yml                 # Jekyll配置文件
├── Gemfile                     # Ruby依赖文件
├── .gitignore                  # Git忽略文件
├── README.md                   # 项目说明文档
├── about/                      # 支队传承部分
│   ├── index.md                # 支队传承主页面
│   ├── mission.md              # 我们的使命
│   ├── timeline.md             # 时间轴
│   ├── members.md              # 成员星群
│   └── handbook.md             # 工作手册
├── species/                    # 物种图鉴部分
│   ├── index.md                # 物种图鉴主页面
│   ├── birds.md                # 鸟类图鉴
│   ├── plants.md               # 植物图鉴
│   └── insects.md              # 昆虫图鉴
├── reports/                    # 调研报告部分
│   ├── index.md                # 调研报告主页面
│   ├── biodiversity.md         # 多样性调研报告
│   ├── ecology.md              # 生态课题调研报告
│   └── humanities.md           # 人文调研报告
├── records/                    # 行程纪实部分
│   ├── index.md                # 行程纪实主页面
│   ├── photos.md               # 摄影集
│   ├── documentary.md          # 纪录片
│   └── creative.md             # 文创周边
├── contact.md                  # 联系我们页面
├── assets/                     # 静态资源
│   ├── css/
│   │   └── style.css           # 全局样式
│   └── images/                 # 图片资源
│       ├── logo.png            # 网站logo
│       ├── banner.jpg          # 横幅图片
│       └── ...                 # 其他图片
└── _includes/                  # Jekyll包含文件
    ├── header.html             # 头部导航
    ├── footer.html             # 页脚
    └── head.html               # HTML头部
```


## 编辑指南

### 编辑现有页面

1. 找到对应的Markdown文件（例如：`about/mission.md`）
2. 使用Markdown语法编辑内容
3. 保存并提交更改

### 添加新页面

1. 在相应目录创建新的Markdown文件（例如：`species/new-bird.md`）
2. 在文件顶部添加YAML front matter：

```yaml
---
layout: page
title: 新鸟类介绍
permalink: /species/new-bird/
---
```

3. 使用Markdown语法编写内容
4. 在导航中添加链接（编辑`_includes/header.html`）

### 本地预览

1. 安装Ruby和Jekyll：`gem install bundler jekyll`
2. 安装依赖：`bundle install`
3. 启动服务器：`bundle exec jekyll serve`
4. 访问 `http://localhost:4000`

## 部署说明

网站通过GitHub Pages自动部署，推送更改到main分支后会自动更新。

## 贡献指南

欢迎所有支队成员贡献内容！
