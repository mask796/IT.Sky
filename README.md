# IT小卖铺

> Windows/Office KMS 激活脚本生成器 · 系统镜像下载 · 修复工具 · 软件导航

## 功能概览

| 模块 | 说明 |
|------|------|
| 🔄 KMS激活 | 一键生成 Windows/Office 批量激活脚本 |
| 💿 系统镜像 | Win11/Win10/Server/Linux 官方镜像下载 |
| 🔧 修复工具 | 清除激活、深度清理C盘等系统维护脚本 |
| 📦 软件导航 | 浏览器、AI、开发、办公等常用软件合集 |
| ⚙️ 管理后台 | 应用/镜像/工具管理、数据导入导出 |

## 技术栈

- **HTML5 + CSS3** — 响应式布局，CSS变量主题
- **原生 JavaScript (ES6+)** — 无框架依赖
- **Font Awesome 6** — 图标库
- **localStorage** — 本地数据持久化

## 文件结构

```
ITXMP/
├── index.html              # 首页（主入口）
├── admin.html              # 管理后台（隐藏入口）
├── iso-intro.html          # 镜像总览页
├── win11-26h1.html         # Windows 11 26H1 详情
├── win11-25h2.html         # Windows 11 25H2 详情
├── win11-24h2.html         # Windows 11 24H2 详情
├── win11-ltsc2024.html     # Win11 LTSC 2024 详情
├── win10-22h2.html         # Windows 10 22H2 详情
├── win10-ltsc2021.html     # Win10 LTSC 2021 详情
├── win7-sp1.html           # Windows 7 SP1 详情
├── server-2025.html        # Windows Server 2025 详情
├── server-2022.html        # Windows Server 2022 详情
├── ubuntu-2404.html        # Ubuntu 24.04 LTS 详情
├── debian-12.html          # Debian 12 详情
├── centos-stream9.html     # CentOS Stream 9 详情
├── rocky-linux9.html       # Rocky Linux 9 详情
├── CODE_WIKI.md            # 代码维基文档
└── .htaccess               # Apache 配置
```

## 快速开始

### 部署方式

**方式一：直接打开**
```bash
# 双击 index.html 即可在浏览器中使用
```

**方式二：本地服务器**
```bash
# PHP内置服务器
php -S localhost:8080

# Python
python -m http.server 8080

# Node.js
npx serve .
```

**方式三：部署到服务器**
- 上传整个 `ITXMP` 目录到 Web 服务器
- 支持 Apache / Nginx / 静态托管（GitHub Pages / Vercel / Netlify）

## 管理后台

### 入口位置
首页页脚 → **「请支持正版软件」**（隐藏链接，新标签页打开）

### 功能模块

#### 📊 仪表盘
- 应用总数 / 镜像数 / 工具数 / 自定义应用 统计

#### 📦 应用管理
- 查看/搜索所有应用（含真实Logo）
- **添加**自定义应用（名称、链接、分类、Logo、描述）
- **编辑**应用信息
- **隐藏/显示**应用（内置和自定义均可）
- **删除**自定义应用

#### 💿 镜像管理
- 查看系统镜像列表及版本详情
- **添加**自定义镜像（名称、描述、版本列表）
- **编辑**自定义镜像
- **隐藏/显示**镜像
- **删除**自定义镜像

#### 🔧 修复工具
- 查看内置修复脚本
- **添加**自定义工具（名称、类型BAT/PS1/VBS/CMD/REG、描述、脚本内容）
- **编辑**自定义工具
- **隐藏/显示**工具
- **查看**脚本内容预览
- **删除**自定义工具

#### 💾 数据管理
- **导出备份**：JSON格式，包含全部自定义数据和应用设置/隐藏状态
- **导入恢复**：兼容 v3.0 格式，自动去重合并
- **清除全部**：重置所有自定义配置

## 数据存储

所有数据通过浏览器 `localStorage` 本地存储：

| Key | 内容 |
|-----|------|
| `it-shop-custom-apps` | 自定义应用列表 |
| `it-shop-app-settings` | 应用设置（隐藏状态、覆盖修改） |
| `it-shop-custom-isos` | 自定义镜像 |
| `it-shop-custom-tools` | 自定义工具 |
| `it-shop-iso-hidden` | 镜像隐藏ID列表 |
| `it-shop-tool-hidden` | 工具隐藏ID列表 |

> 数据仅在当前浏览器生效，换浏览器或清除缓存会丢失，请定期导出备份。

## 浏览器兼容性

| 浏览器 | 版本 |
|--------|------|
| Chrome | 90+ |
| Edge | 90+ |
| Firefox | 88+ |
| Safari | 14+ |

## 许可声明

仅供学习使用 · 请支持正版软件

© 2024 IT小卖铺
