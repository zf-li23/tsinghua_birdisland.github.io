# tsinghua_birdisland.github.io

清华大学“鸟岛与少年”实践支队官方网站  
展示支队生态保护成果、成员风采与调研纪实。

---

## 目录结构

```
tsinghua_birdisland.github.io/
├── index.html                  # 网站首页（Jekyll，layout: home）
├── _config.yml                 # Jekyll 配置文件（含 baseurl 设置）
├── Gemfile                     # Ruby 依赖
├── .gitignore                  # Git忽略文件
├── assets/
│   ├── css/
│   │   ├── style.css           # 全局样式
│   │   └── style_home.css      # 首页样式
│   └── images/                 # 图片资源
├── _layouts/                   # Jekyll 页面布局
│   ├── default.html
│   └── home.html
├── _includes/                  # 可复用片段
│   ├── header.html             # 通用页眉
│   ├── header_home.html        # 首页专用页眉
│   └── footer.html             # 页脚
├── README.md                   # 项目说明文档
├── about/                      # 支队传承相关页面
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
└── contact.md                  # 联系我们页面
```

---

## 使用说明

### 1. 预览
访问`[鸟岛与少年](https://zf-li23.github.io/tsinghua_birdisland.github.io/)`

### 2. 编辑内容

- **首页**：编辑 `index.html`，使用 `layout: home`
- **栏目页**：在对应目录（如 `about/`）下编辑 `.md` 文件，YAML 头部指定 `layout: default`
- **导航与页眉/页脚**：修改 `_includes/header.html`、`header_home.html`、`footer.html`
- **样式**：编辑 `assets/css/style.css` 或 `style_home.css`

### 3. 插入图片

- 将图片放入 `assets/images/` 目录（如需新建请自行创建）
- 在 Markdown 或 HTML 中引用图片：
  ```markdown
  ![描述]({{ '/assets/images/图片名.jpg' | relative_url }})
  ```
  或
  ```html
  <img src="{{ '/assets/images/图片名.jpg' | relative_url }}" alt="描述">
  ```

### 4. 路径与 baseurl

- 所有资源和链接请使用 `{{ '/路径/' | relative_url }}` 或 `{{ site.baseurl }}`，确保在 GitHub Pages 子路径下正常访问。

---

## 部署说明

- 推送到 GitHub 仓库的 `main` 分支后，GitHub Pages 会自动构建并发布到  
  `https://zf-li23.github.io/tsinghua_birdisland.github.io/`

---

## 贡献与维护

- 欢迎支队成员共同维护和完善内容。
- 编辑内容请遵循 Markdown 语法和 Jekyll 约定。
- 如有问题可通过 Issues 反馈。
