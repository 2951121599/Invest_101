# Docsify 部署说明

本项目使用 Docsify 进行文档部署。

## GitHub Pages 配置

### 1. 启用 GitHub Pages

1. 访问仓库设置：`https://github.com/2951121599/Invest_101/settings/pages`
2. 在 **Source** 部分：
   - 选择 **Deploy from a branch**
   - **Branch** 选择 `main`
   - **Folder** 选择 `/ (root)`
3. 点击 **Save**

### 2. 访问地址

配置完成后，访问地址为：
- `https://2951121599.github.io/Invest_101/`

### 3. 等待构建

- GitHub Pages 通常需要 1-2 分钟构建
- 构建完成后即可访问

## 本地预览

### 安装 Docsify CLI

```bash
npm i docsify-cli -g
```

### 启动本地服务器

```bash
docsify serve .
```

然后访问 `http://localhost:3000`

## 项目结构

```
Invest_101/
├── index.html          # Docsify 入口文件
├── _sidebar.md         # 侧边栏导航
├── _404.md            # 404 错误页面
├── README.md          # 首页内容
├── docs/              # 文档目录
├── tools/             # 工具文件
├── resources/         # 学习资源
└── examples/          # 案例研究
```

## 自定义配置

编辑 `index.html` 中的 `window.$docsify` 对象可以自定义配置：

- `name`: 网站名称
- `repo`: GitHub 仓库地址
- `loadSidebar`: 是否加载侧边栏
- `search`: 搜索配置
- `pagination`: 分页配置

更多配置选项请参考 [Docsify 官方文档](https://docsify.js.org/#/configuration)

