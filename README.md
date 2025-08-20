# EdgeOne Pages Next.js Starter - 混合渲染演示

在 EdgeOne Pages 上使用 Next.js 来构建高性能、可扩展的Web应用。演示 SSR、ISR、SSG、Streaming、Node Functions 和 Edge Functions。

## ✨ 项目特性

### 🔄 混合渲染策略
- **SSR (服务器端渲染)** - 每次请求后通过服务器实时渲染
- **ISR (增量静态再生)** - 静态生成 + 定时增量更新
- **SSG (静态站点生成)** - 在构建时预生成所有页面
- **Streaming (流式渲染)** - 逐步渲染页面内容，提升用户体验

### 🚀 运行时支持
- **Node Functions** - 在 Node.js 运行时运行代码，支持完整的 Node.js API
- **Edge Functions** - 在边缘运行时运行代码，提供最低延迟的全球部署

### 🎨 设计特色
- **黑底白字主题** - 现代化的深色设计风格
- **蓝色点缀色** - 使用 `#1c66e5` 作为主要强调色
- **响应式布局** - 完美适配各种设备尺寸
- **流畅动画** - 优雅的过渡效果和加载动画

## 🛠️ 技术实现

### 核心技术栈
- **Next.js 15** - 最新的 App Router 架构
- **React 19** - 最新的 React 特性
- **TypeScript** - 完整的类型安全
- **Tailwind CSS v4** - 现代化的 CSS 框架
- **shadcn/ui** - 高质量的可复用组件

### 架构特点
- **App Router** - 基于文件系统的路由
- **Server Components** - 默认服务器端渲染
- **Client Components** - 按需客户端交互
- **API Routes** - 内置 API 端点支持
- **Streaming** - 渐进式内容加载

## 📁 项目结构

```
next-mix-template/
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   ├── hello/route.ts      # Node.js API 示例
│   │   │   └── edge/route.ts       # Edge API 示例
│   │   ├── ssr/page.tsx            # SSR 演示页面
│   │   ├── isr/page.tsx            # ISR 演示页面
│   │   ├── ssg/page.tsx            # SSG 演示页面
│   │   ├── streaming/page.tsx      # Streaming 演示页面
│   │   ├── node-functions/page.tsx # Node Functions 演示
│   │   ├── edge-functions/page.tsx # Edge Functions 演示
│   │   ├── layout.tsx              # 根布局组件
│   │   └── page.tsx                # 首页
│   ├── components/
│   │   ├── ui/                     # shadcn/ui 组件
│   │   ├── Header.tsx              # 导航头部
│   │   ├── Hero.tsx                # 英雄区域
│   │   ├── FeatureCard.tsx         # 特性卡片
│   │   └── Features.tsx            # 特性展示
│   └── lib/
│       └── utils.ts                # 工具函数
├── public/                          # 静态资源
├── tailwind.config.ts              # Tailwind 配置
├── components.json                  # shadcn/ui 配置
└── package.json                     # 项目依赖
```

## 🚀 快速开始

### 环境要求
- Node.js 18+ 
- npm 或 yarn

### 安装依赖
```bash
npm install
```

### 启动开发服务器
```bash
npm run dev
```

### 构建生产版本
```bash
npm run build
npm start
```

## 🌐 访问地址

- **首页**: `http://localhost:3000`
- **SSR**: `http://localhost:3000/ssr`
- **ISR**: `http://localhost:3000/isr`
- **SSG**: `http://localhost:3000/ssg`
- **Streaming**: `http://localhost:3000/streaming`
- **Node Functions**: `http://localhost:3000/node-functions`
- **Edge Functions**: `http://localhost:3000/edge-functions`

## 🔌 API 端点

### Node.js Runtime
- **GET/POST** `/api/hello` - 演示 Node.js 运行时特性

### Edge Runtime
- **GET/POST** `/api/edge` - 演示边缘运行时特性

## 📚 功能详解

### SSR (服务器端渲染)
- 每次请求后通过服务器实时渲染
- 确保内容始终是最新的
- 适合动态内容和个性化页面

### ISR (增量静态再生)
- 静态生成 + 定时增量更新
- 平衡性能和内容新鲜度
- 适合博客、新闻等定期更新的内容

### SSG (静态站点生成)
- 在构建时预生成所有页面
- 提供最快的加载速度
- 适合企业官网、文档等静态内容

### Streaming (流式渲染)
- 逐步渲染页面内容
- 提升用户体验和感知性能
- 支持大型页面和复杂内容

### Node Functions
- 完整的 Node.js API 支持
- 支持所有 npm 包
- 适合复杂业务逻辑和数据处理

### Edge Functions
- 全球边缘部署
- 超低延迟响应
- 适合实时数据处理和地理位置服务

## 🎨 自定义配置

### 主题颜色
在 `tailwind.config.ts` 中修改主色调：
```typescript
colors: {
  primary: "#1c66e5", // 自定义主色调
}
```

### 组件样式
在 `src/app/globals.css` 中自定义全局样式：
```css
body {
  background: #000000;  // 自定义背景色
  color: #ffffff;       // 自定义文字色
}
```

## 📖 学习资源

- [Next.js 官方文档](https://nextjs.org/docs)
- [React 官方文档](https://react.dev/)
- [Tailwind CSS 文档](https://tailwindcss.com/docs)
- [shadcn/ui 组件库](https://ui.shadcn.com/)

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request 来改进这个项目！

## 📄 许可证

MIT License

---

**享受构建高性能 Web 应用的乐趣！** 🚀
