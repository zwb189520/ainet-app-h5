# ainet-app-h5

一个移动端 H5 App 演示原型，主要用于展示家庭设备、日程、清单、任务、图库、设备管理等 App 页面与交互流程。

## 项目简介

本项目是纯前端静态页面 Demo，入口文件为 `index.html`。页面样式、交互逻辑和模拟数据均内置在单个 HTML 文件中，不依赖后端接口，也不需要构建工具。

适合用于：

- App 页面视觉还原与流程演示
- 产品原型交互走查
- 移动端 H5 静态预览
- 设备管理、家庭管理、日程清单等功能演示

## 功能模块

- 登录、验证码登录、重置密码等账号流程
- 首页设备展示与设备入口
- Smart Calendar、AI Calendar、Smart Clock、墨水屏相框等设备展示
- 日程、清单、任务页面
- 图库、AI 生成风格选择、图片发送到设备等流程
- 添加设备、扫描设备、设备属性、设备升级
- 设置、家庭管理、成员选择等页面
- 弹窗、Toast、Tab、筛选、表单输入等基础交互

## 目录结构

```text
.
├── index.html                 # H5 Demo 主入口，包含页面、样式、脚本和模拟数据
├── files/                     # Lottie/JSON 动画资源
├── image/                     # 图片与图标资源
│   └── product_images/        # 产品设备图片
├── agent.md                   # 开发协作说明
└── README.md                  # 项目说明
```

## 本地预览

方式一：直接打开

```text
index.html
```

方式二：使用任意静态服务器预览，例如：

```bash
python -m http.server 8080
```

然后在浏览器访问：

```text
http://localhost:8080
```

## 技术说明

- 原生 HTML、CSS、JavaScript 实现
- 移动端优先布局
- 使用 hash/前端状态模拟页面跳转
- 所有业务数据均为前端模拟数据
- 不连接真实后端服务
- 不依赖 npm、webpack、vite 等构建工具

## 资源说明

- `image/`：页面图标、头像、设备图片等静态图片
- `files/`：页面中使用的动画 JSON 资源
- `index.html`：包含完整页面结构、样式、脚本和交互逻辑

## 部署

该项目为纯静态页面，可直接部署到任意静态托管服务，例如 GitHub Pages、Nginx、OSS/CDN 或其他静态网站服务。

部署时保留以下文件和目录即可：

```text
index.html
files/
image/
```
