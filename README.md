# Vers123 游戏导航网站

一个简洁美观的游戏导航网站，提供米哈游(miHoYo)游戏和其他热门游戏的官方导航链接。

![项目状态](https://img.shields.io/badge/状态-维护中-success)
![License](https://img.shields.io/badge/许可证-MIT-blue)
![HTML5](https://img.shields.io/badge/HTML5-最新版本-orange)
![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.x-38bdf8)

## 📋 目录

- [项目简介](#项目简介)
- [功能特性](#功能特性)
- [项目结构](#项目结构)
- [快速开始](#快速开始)
- [使用方法](#使用方法)
- [技术栈](#技术栈)
- [游戏列表](#游戏列表)
- [开发指南](#开发指南)
- [SEO优化](#seo优化)
- [性能优化](#性能优化)
- [常见问题](#常见问题)
- [更新日志](#更新日志)
- [贡献指南](#贡献指南)
- [许可证](#许可证)
- [联系方式](#联系方式)

## 项目简介

本项目是一个静态网页导航站点，帮助用户快速访问各种游戏的官方网站。采用现代化的响应式设计，为用户提供流畅的浏览体验。

### 导航分类

- **miHoYo 导航** - 米哈游旗下游戏官网导航
- **Another Game 导航** - 其他热门游戏导航

### 项目亮点

- 🎨 **现代化设计** - 采用 Tailwind CSS 构建精美界面
- 📱 **完全响应式** - 完美适配桌面、平板和移动设备
- ⚡ **快速加载** - 优化的资源加载，提供极速访问体验
- 🔍 **SEO友好** - 内置搜索引擎优化配置
- 🎯 **用户友好** - 直观的导航结构和交互设计

## 功能特性

### 核心功能

- ✅ 响应式设计，支持桌面和移动设备
- ✅ 简洁的侧边栏导航菜单
- ✅ 优雅的卡片式布局展示游戏
- ✅ 点击交互效果（替代悬停效果，提升移动端体验）
- ✅ 使用 Tailwind CSS 进行样式设计
- ✅ Font Awesome 图标库

### 交互体验

- 🖱️ 点击切换内容区域
- 🎯 清晰的游戏分类展示
- 🌈 平滑的过渡动画效果
- 📋 便捷的官方链接跳转

## 项目结构

```
vers123.github.io/
├── index.html                          # 主页导航入口
├── README.md                           # 项目说明文档
└── Web/
    ├── mihoyo_web/
    │   ├── miHoYo.html                 # 米哈游游戏导航页
    │   └── mihoyo/
    │       └── images/
    │           ├── game_logo/          # 游戏Logo图片
    │           │   ├── Genshin Impact.jpg
    │           │   ├── Honkai Star Rail.jpg
    │           │   ├── Zenless Zone Zero.jpg
    │           │   ├── Star Valley.jpg
    │           │   ├── honkai_nexus_anima.jpg
    │           │   ├── Honkai Impact 3rd.jpg
    │           │   ├── Tears of Themis.jpg
    │           │   └── Guns Girl Z.jpg
    │           └── logo/               # 米哈游Logo图片
    │               └── miHoYo.png
    └── another_game_web/
        ├── another_games.html          # 其他游戏导航页
        └── another_games/
            └── images/
                ├── game_logo/          # 游戏Logo图片
                │   ├── League of Legends.jpg
                │   ├── Valorant.jpg
                │   ├── Apex Legends.jpg
                │   ├── Fortnite.jpg
                │   ├── Minecraft.jpg
                │   └── Overwatch 2.jpg
                └── logo/               # Logo图片
                    └── another_games.png
```

## 快速开始

### 环境要求

- 现代浏览器（Chrome、Firefox、Safari、Edge）
- 网络连接（用于加载CDN资源）

### 本地预览

1. **克隆项目**
   ```bash
   git clone https://github.com/vers123/vers123.github.io.git
   cd vers123.github.io
   ```

2. **直接打开**
   - 双击 `index.html` 文件，使用浏览器打开
   - 或右键选择"打开方式" > 选择浏览器

3. **使用本地服务器（可选）**
   ```bash
   # 使用 Python 3
   python -m http.server 8000
   
   # 使用 Node.js (需要安装 http-server)
   npx http-server -p 8000
   ```
   然后在浏览器访问 `http://localhost:8000`

### 部署到 GitHub Pages

1. **推送到 GitHub**
   ```bash
   git add .
   git commit -m "Initial commit"
   git push origin main
   ```

2. **启用 GitHub Pages**
   - 进入仓库 Settings > Pages
   - Source 选择 "Deploy from a branch"
   - Branch 选择 `main` (或 `master`)
   - Folder 选择 `/ (root)`
   - 点击 Save

3. **访问网站**
   - 等待部署完成后，访问 `https://yourusername.github.io/vers123.github.io`
   - 或 `https://yourusername.github.io/` (如果仓库名为 `yourusername.github.io`)

## 使用方法

### 导航使用

1. **主页导航**
   - 打开 `index.html` 查看导航入口
   - 点击对应分类进入详细页面

2. **游戏导航页**
   - 使用左侧菜单切换游戏分类
   - 点击游戏卡片访问官方网站
   - 浏览游戏简介和类型信息

### 自定义配置

#### 添加新游戏

在对应的 HTML 文件中找到游戏卡片区域，添加新的卡片：

```html
<a href="游戏官网链接" target="_blank" title="游戏名称">
  <img src="图片路径" alt="游戏名称" class="h-20 md:h-24 lg:h-32 w-auto object-cover">
  <div class="p-4">
    <h3 class="text-xl font-semibold text-gray-800">游戏名称</h3>
    <p class="text-gray-600 text-sm mt-1">游戏类型描述</p>
  </div>
</a>
```

#### 修改样式

项目使用 Tailwind CSS，可以通过修改 class 属性来自定义样式：

- 颜色：`text-gray-800`、`bg-blue-500` 等
- 间距：`p-4`、`m-2` 等
- 尺寸：`h-20`、`w-auto` 等
- 响应式：`md:h-24`、`lg:h-32` 等

## 技术栈

### 前端技术

- **HTML5** - 页面结构和语义化标签
- **Tailwind CSS 3.x** - 实用优先的CSS框架（通过CDN引入）
- **Font Awesome 4.7** - 图标库（通过CDN引入）
- **JavaScript (ES6+)** - 交互功能和动态内容切换

### 设计理念

- **移动优先** - 从小屏幕开始设计，逐步适配大屏幕
- **渐进增强** - 基础功能在所有浏览器可用，高级功能在支持浏览器中增强
- **性能优先** - 最小化资源加载，优化渲染性能

## 游戏列表

### miHoYo 游戏导航

| 游戏名称 | 类型 | 官网链接 |
|---------|------|---------|
| 原神 | 开放世界冒险 | [官网](https://genshin.hoyoverse.com) |
| 崩坏：星穹铁道 | 回合制角色扮演 | [官网](https://sr.mihoyo.com/main) |
| 绝区零 | 动作角色扮演 | [官网](https://zenless.hoyoverse.com) |
| 星布谷地 | 模拟经营 | [官网](https://www.hoyoverse.com) |
| 崩坏：因缘精灵 | 策略卡牌 | [官网](https://www.hoyoverse.com) |
| 崩坏3 | 3D动作射击 | [官网](https://honkai3rd.hoyoverse.com) |
| 未定事件簿 | 恋爱推理 | [官网](https://tearsofthemis.hoyoverse.com) |
| 崩坏学园2 | 2D动作射击 | [官网](https://www.hoyoverse.com) |

### 米游社平台

| 平台名称 | 功能 | 官网链接 |
|---------|------|---------|
| 米游社官网 | 游戏社区 | [官网](https://bbs.mihoyo.com) |
| 米游社-大别墅 | 创作者平台 | [官网](https://www.miyoushe.com) |

### Another Game 导航

| 游戏名称 | 类型 | 官网链接 |
|---------|------|---------|
| 英雄联盟 | MOBA | [官网](https://lol.qq.com) |
| 无畏契约 | 战术射击 | [官网](https://valorant.qq.com) |
| Apex 英雄 | 大逃杀 | [官网](https://www.ea.com/zh-cn/games/apex-legends) |
| 堡垒之夜 | 大逃杀 | [官网](https://www.epicgames.com/fortnite) |
| 我的世界 | 沙盒建造 | [官网](https://www.minecraft.net) |
| 守望先锋2 | 团队射击 | [官网](https://overwatch.blizzard.com) |

## 开发指南

### 代码规范

#### HTML 规范

- 使用语义化标签（`header`、`nav`、`main`、`footer`）
- 所有标签必须正确闭合
- 图片必须包含 `alt` 属性
- 链接使用 `target="_blank"` 时建议添加 `rel="noopener noreferrer"`

#### CSS 规范

- 优先使用 Tailwind CSS 实用类
- 自定义样式放在 `<style>` 标签内
- 保持类名简洁明了
- 遵循移动优先原则

#### JavaScript 规范

- 使用 `const` 和 `let` 代替 `var`
- 函数使用箭头函数或传统函数声明
- 事件处理使用 `addEventListener` 或内联事件
- 保持代码简洁，避免冗余逻辑

### 调试技巧

1. **浏览器开发者工具**
   - F12 打开开发者工具
   - 使用 Elements 面板检查 HTML 和 CSS
   - 使用 Console 面板查看 JavaScript 错误
   - 使用 Network 面板检查资源加载

2. **响应式测试**
   - 使用开发者工具的设备模拟模式
   - 测试不同屏幕尺寸（320px、768px、1024px、1920px）
   - 检查移动端和桌面端的显示效果

3. **性能测试**
   - 使用 Lighthouse 进行性能评分
   - 检查资源加载时间
   - 优化图片大小和格式

## SEO优化

### 已实现的优化

- ✅ Meta 描述标签
- ✅ Meta 关键词标签
- ✅ 作者信息标签
- ✅ 语义化 HTML 结构
- ✅ 图片 alt 属性
- ✅ 友好的 URL 结构

### Meta 标签示例

```html
<meta name="description" content="Vers123 游戏导航网站 - 提供米哈游(miHoYo)游戏和其他热门游戏的官方导航链接">
<meta name="keywords" content="游戏导航,米哈游,原神,崩坏星穹铁道,游戏官网,游戏链接">
<meta name="author" content="Vers123">
```

### SEO 建议

1. **定期更新内容** - 保持游戏信息的时效性
2. **优化图片** - 使用合适的文件格式和压缩
3. **提升加载速度** - 优化资源加载顺序
4. **建立外链** - 增加网站的外部链接
5. **提交搜索引擎** - 向 Google、百度等提交网站

## 性能优化

### 已实现的优化

- ✅ CDN 加载外部资源
- ✅ 响应式图片
- ✅ 最小化 JavaScript
- ✅ CSS 实用类优先
- ✅ 避免不必要的 DOM 操作

### 性能指标

- **首次内容绘制 (FCP)**: < 1.5s
- **最大内容绘制 (LCP)**: < 2.5s
- **首次输入延迟 (FID)**: < 100ms
- **累积布局偏移 (CLS)**: < 0.1

### 优化建议

1. **图片优化**
   - 使用 WebP 格式
   - 压缩图片大小
   - 使用懒加载（`loading="lazy"`）

2. **代码优化**
   - 压缩 HTML、CSS、JavaScript
   - 移除未使用的代码
   - 使用代码分割

3. **缓存策略**
   - 设置合适的缓存头
   - 使用 Service Worker
   - 利用浏览器缓存

## 常见问题

### Q: 为什么有些图片无法显示？

A: 请检查以下几点：
- 确认图片路径是否正确
- 检查图片文件是否存在
- 确认图片格式是否支持
- 检查网络连接是否正常

### Q: 如何添加新的游戏？

A: 按照以下步骤操作：
1. 准备游戏 Logo 图片，放入对应的 `game_logo` 文件夹
2. 在 HTML 文件中找到游戏卡片区域
3. 复制现有的卡片代码
4. 修改链接、图片路径、游戏名称和描述

### Q: 如何修改网站主题颜色？

A: Tailwind CSS 使用类名控制样式，可以：
1. 修改颜色类名（如 `text-blue-500` 改为 `text-red-500`）
2. 在 `<style>` 标签中添加自定义样式
3. 使用 CSS 变量进行主题切换

### Q: 网站支持哪些浏览器？

A: 本网站支持以下现代浏览器：
- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

不支持 IE 浏览器。

### Q: 如何在移动设备上获得最佳体验？

A: 建议：
- 使用 Chrome 或 Safari 浏览器
- 确保网络连接稳定
- 横屏浏览可以获得更好的显示效果

## 更新日志

### v1.0 (2025-12-23)

- � 项目首次发布
- ✨ 创建主页导航入口页面
- ✨ 实现 miHoYo 游戏导航页面
- ✨ 实现 Another Game 导航页面
- ✨ 实现响应式设计，支持桌面和移动设备
- ✨ 添加 Font Awesome 图标
- ✨ 使用 Tailwind CSS 构建精美界面
- ✨ 添加侧边栏导航菜单
- ✨ 实现点击切换内容区域的交互功能
- ✨ 添加 SEO 优化（meta 标签）
- ✨ 创建详细的 README 文档
- ✅ 完成项目验证和测试

---

<div align="center">

**如果这个项目对你有帮助，请给一个 ⭐️**

Made with ❤️ by Vers123

© 2025 Vers123 | 本网站仅作展示用途

</div>
