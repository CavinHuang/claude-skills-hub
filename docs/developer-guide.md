# 开发者指南

本指南为想要参与 Claude Skills Hub 开发的开发者提供详细的技术文档和开发指导。

## 📚 目录

- [环境设置](#环境设置)
- [项目架构](#项目架构)
- [技能开发](#技能开发)
- [API 参考](#api-参考)
- [测试指南](#测试指南)
- [部署流程](#部署流程)

## 🛠️ 环境设置

### 系统要求
- Node.js 18.0+
- npm 8.0+ 或 yarn 1.22+
- Git 2.30+
- Claude Desktop 1.0+

### 本地开发环境

1. **克隆仓库**
```bash
git clone https://github.com/YavinHuang/claude-skills-hub.git
cd claude-skills-hub
```

2. **安装依赖**
```bash
npm install
# 或
yarn install
```

3. **环境配置**
```bash
cp .env.example .env.local
# 编辑 .env.local 文件，配置必要的环境变量
```

4. **启动开发服务器**
```bash
npm run dev
```

5. **访问应用**
打开浏览器访问 [http://localhost:3000](http://localhost:3000)

### 开发工具推荐
- **IDE**: Visual Studio Code
- **插件**: 
  - ES7+ React/Redux/React-Native snippets
  - Prettier - Code formatter
  - ESLint
  - Tailwind CSS IntelliSense

## 🏗️ 项目架构

### 技术栈
- **前端**: Next.js 14, React 18, TypeScript
- **样式**: Tailwind CSS, Framer Motion
- **数据库**: PostgreSQL, Prisma ORM
- **缓存**: Redis
- **部署**: Vercel, AWS

### 目录结构
```
claude-skills-hub/
├── app/                    # Next.js App Router
│   ├── (pages)/           # 页面组件
│   ├── api/               # API 路由
│   └── globals.css        # 全局样式
├── components/            # React 组件
│   ├── ui/               # 基础 UI 组件
│   ├── features/         # 功能组件
│   └── layout/           # 布局组件
├── lib/                  # 工具库
├── types/                # TypeScript 类型定义
├── hooks/                # 自定义 React Hooks
├── utils/                # 工具函数
├── styles/               # 样式文件
├── public/               # 静态资源
├── docs/                 # 文档
└── skills/               # 技能定义
```

### 核心概念

#### 技能模型
```typescript
interface Skill {
  id: string;
  name: string;
  description: string;
  category: SkillCategory;
  tags: string[];
  author: string;
  version: string;
  downloads: number;
  rating: number;
  createdAt: Date;
  updatedAt: Date;
  metadata: SkillMetadata;
}
```

#### 技能类别
```typescript
type SkillCategory = 
  | 'development'
  | 'design'
  | 'business'
  | 'analytics'
  | 'education'
  | 'content'
  | 'research'
  | 'entertainment';
```

## 🎯 技能开发

### 技能结构
每个技能遵循标准化的文件结构：

```
skill-name/
├── SKILL.md          # 技能主文档
├── README.md         # 详细说明
├── LICENSE.txt       # 许可证
├── examples/         # 使用示例
│   ├── basic.md
│   └── advanced.md
├── tests/            # 测试文件
│   └── test.json
├── assets/           # 资源文件
│   └── icon.png
└── config/           # 配置文件
    └── skill.json
```

### 技能元数据
```json
{
  "name": "skill-name",
  "version": "1.0.0",
  "description": "技能描述",
  "category": "development",
  "tags": ["tag1", "tag2"],
  "author": "作者名称",
  "license": "MIT",
  "repository": "https://github.com/author/skill-repo",
  "keywords": ["关键词1", "关键词2"],
  "claude": {
    "minVersion": "1.0.0",
    "maxVersion": "*"
  },
  "dependencies": [],
  "files": [
    "SKILL.md",
    "README.md",
    "examples/"
  ]
}
```

### 技能开发流程

1. **创建技能**
```bash
npm run create-skill <skill-name>
```

2. **编写技能文档**
编辑 `SKILL.md` 文件，包含完整的技能说明

3. **创建示例**
在 `examples/` 目录下创建使用示例

4. **添加测试**
在 `tests/` 目录下添加测试文件

5. **本地测试**
```bash
npm run test:skill <skill-name>
```

6. **提交审核**
```bash
git add .
git commit -m "feat: add new skill <skill-name>"
git push origin feature/new-skill
```

## 🔌 API 参考

### REST API

#### 获取技能列表
```http
GET /api/skills
```

查询参数：
- `category`: 技能类别
- `search`: 搜索关键词
- `page`: 页码
- `limit`: 每页数量
- `sort`: 排序方式

#### 获取技能详情
```http
GET /api/skills/{id}
```

#### 安装技能
```http
POST /api/skills/{id}/install
```

### GraphQL API

#### 查询技能
```graphql
query GetSkills($category: String, $search: String) {
  skills(category: $category, search: $search) {
    id
    name
    description
    category
    tags
    downloads
    rating
  }
}
```

## 🧪 测试指南

### 单元测试
```bash
npm run test
```

### 集成测试
```bash
npm run test:integration
```

### E2E 测试
```bash
npm run test:e2e
```

### 测试覆盖率
```bash
npm run test:coverage
```

### 技能测试
```bash
npm run test:skill <skill-name>
```

## 🚀 部署流程

### 预提交检查
```bash
npm run lint
npm run test
npm run build
```

### 构建项目
```bash
npm run build
```

### 部署到 Vercel
```bash
vercel --prod
```

### 数据库迁移
```bash
npm run db:migrate
```

## 📝 贡献指南

详细的贡献指南请参考 [CONTRIBUTING.md](../CONTRIBUTING.md)

### 代码规范
- 使用 ESLint 和 Prettier
- 遵循 TypeScript 严格模式
- 编写单元测试
- 添加 JSDoc 注释

### 提交规范
使用 Conventional Commits 规范：
```
feat: 新功能
fix: 修复问题
docs: 文档更新
style: 代码格式调整
refactor: 代码重构
test: 测试相关
chore: 构建工具或辅助工具的变动
```

## 🤝 社区

- **GitHub**: [项目仓库](https://github.com/CavinHuang/claude-skills-hub)
- **Discussions**: [讨论区](https://github.com/CavinHuang/claude-skills-hub/discussions)
- **Issues**: [问题跟踪](https://github.com/CavinHuang/claude-skills-hub/issues)

## 📞 获取帮助

如果您在开发过程中遇到问题：

- **📧 开发者邮件**: [dev@claudeskill.site](mailto:dev@claudeskill.site)
- **💬 Discord**: [开发者社区](https://discord.gg/claudeskills)
- **📖 文档**: [完整文档](https://docs.claudeskill.site)

---

欢迎贡献代码！🎉
