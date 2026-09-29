# APX — Pipeline Exchange

APX 是一个面向生物医药资产管线交易与撮合的轻量级单页应用（SPA）。

## 特性

- **全功能单页应用**: 无外部重型框架依赖，极速加载与流畅交互。
- **角色切换与看板**: 支持买方（Buyer）、卖方（Seller）及访客模式，内置管线资产库、筛选、匹配与关注清单。
- **开箱即用**: 支持静态托管，无需服务端渲染或复杂构建流程。

## 本地预览

直接在浏览器中打开 `index.html`，或使用任意本地静态服务器：

```bash
# 使用 Python
python3 -m http.server 3000

# 或使用 npx serve
npx serve .
```

打开浏览器访问 `http://localhost:3000` 即可。

## Vercel 部署

本项目已配置 `vercel.json`，支持一键部署到 Vercel：

### 方式一：GitHub 导入（推荐）

1. 登录 [Vercel 控制台](https://vercel.com)。
2. 点击 **Add New...** -> **Project**。
3. 从 GitHub 仓库列表中选择 `apx` 仓库并点击 **Import**。
4. Framework Preset 保持为 **Other**，Root Directory 保持为 `./`，直接点击 **Deploy**。
5. 部署完成后即可获得生产访问链接。后续每次向 `main` 分支推代码均会自动触发持续部署。

### 方式二：使用 Vercel CLI

```bash
# 全局安装 Vercel CLI（若尚未安装）
npm i -g vercel

# 在项目根目录下执行部署
vercel

# 部署至生产环境
vercel --prod
```
