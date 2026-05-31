# 暖爪宠物洗护单页网站

一个面向宠物洗护门店的中文 HTML 单页网站。页面以预约转化为核心，包含服务介绍、护理流程、套餐价格、店内环境轮播、客户评价和预约表单。

## 功能亮点

- 原生 HTML、CSS 和 JavaScript 实现，无需构建工具。
- 响应式布局，适配桌面、平板和手机浏览。
- 店内环境轮播展示三个区域：接待等候区、犬只洗护区、猫咪安静护理区。
- 预约表单包含基础必填校验，提交后显示前端成功提示。
- 图片资产已放入本地 `assets/` 目录，核心页面不依赖额外框架。

## 项目结构

```text
.
├── index.html
├── assets/
│   ├── interior-cat-room.png
│   ├── interior-grooming.png
│   └── interior-reception.png
├── .gitignore
└── README.md
```

## 本地预览

可以直接用浏览器打开 `index.html`。如果希望用本地服务预览，进入项目目录后运行：

```bash
python3 -m http.server 4173 --bind 127.0.0.1
```

然后访问：

```text
http://127.0.0.1:4173/
```

## 主要内容位置

- 页面结构、样式和交互都在 `index.html` 中。
- 店内环境轮播图片位于 `assets/`。
- 轮播逻辑使用 `data-carousel`、`data-slide`、`data-carousel-dot` 等属性绑定。
- 预约表单逻辑绑定在 `#bookingForm`。

## 维护说明

- 修改门店名称、电话、地址、营业时间时，直接搜索对应中文内容并替换。
- 替换轮播图片时，建议保持 16:9 横图比例，并更新对应 `alt` 文案。
- 新增本地资源时，优先放入 `assets/`。
- 不要提交系统文件、编辑器配置、依赖目录、构建产物、日志、环境变量或临时缓存；这些已在 `.gitignore` 中排除。

## Git

当前项目已初始化为 Git 工程，主分支为 `main`，远端仓库为：

```text
git@github.com:KsongloveCv/pet_care.git
```
