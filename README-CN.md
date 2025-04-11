# 产品经理个人博客 - 基于NotionNext

这是一个基于NotionNext的个人博客项目，专为互联网软件&AI方向的产品经理设计。

## 特点

- 使用Notion作为CMS，轻松管理博客内容
- 支持文章、项目展示、个人介绍等内容
- 简洁现代的设计风格
- 响应式布局，适配各种设备
- 支持暗色模式
- 集成社交媒体链接
- SEO友好

## 本地开发

1. 克隆仓库
```bash
git clone https://github.com/你的用户名/你的仓库名.git
```

2. 安装依赖
```bash
cd 你的仓库名
npm install
```

3. 配置环境变量
   - 复制`.env.example`为`.env`
   - 编辑`.env`文件，填入你的Notion API密钥和数据库ID

4. 启动开发服务器
```bash
npm run dev
```

## Notion设置

1. 创建Notion集成
   - 访问[Notion Developers](https://www.notion.so/my-integrations)
   - 创建新的集成，获取API密钥

2. 创建博客数据库
   - 创建全页面数据库
   - 添加必要的属性列：title, date, tags, category, status, slug, summary
   - 将你的Notion集成添加为数据库的共享成员

3. 数据库ID
   - 从数据库URL中获取ID：https://www.notion.so/xxxxx?v=xxxx
   - ID是第一个问号前的字符串部分

## 部署到Vercel

1. 在GitHub上创建仓库并推送代码
2. 在[Vercel](https://vercel.com)中导入该仓库
3. 配置环境变量：
   - `NOTION_PAGE_ID` (必须)
   - `NOTION_API_SECRET` (必须)
   - 其他自定义配置项
4. 部署应用

## 自定义

- 主题: 修改`.env`文件中的`NEXT_PUBLIC_THEME`
- 个人信息: 修改`.env`文件中的作者、简介等信息
- 社交媒体: 添加你的社交媒体链接
- 欢迎语: 修改`NEXT_PUBLIC_GREETING_WORDS`

## 许可证

MIT 