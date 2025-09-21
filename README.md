# 学友社（LearnHub）学习论坛

学友社是一个专注于学习交流的在线论坛平台，旨在为不同领域的学习者提供知识分享、问题解答和互动学习的空间。

## 技术架构

### 后端技术栈
- **框架**: Django 4.2 LTS + Django REST Framework 3.14+
- **数据库**: PostgreSQL 14+
- **缓存**: Redis 7.0+
- **认证**: Django Simple JWT 5.2+
- **搜索**: Elasticsearch 8.0+ (可选)
- **任务队列**: Celery 5.2+

### 前端技术栈
- **框架**: Vue.js 3.3+
- **构建工具**: Vite 4.0+
- **状态管理**: Pinia 2.1+
- **UI 组件库**: Element Plus 2.3+
- **富文本编辑器**: TinyMCE 6.0+

## 核心功能

### 用户系统
- 用户注册和登录
- 个人资料管理
- 积分和等级系统
- 徽章奖励机制
- 学习目标管理

### 论坛功能
- 版块分类管理
- 帖子发布和编辑
- 评论和回复系统
- 点赞和收藏功能
- 全文搜索

### 互动功能
- 用户关注系统
- 私信功能
- 通知系统
- 举报和审核

### 管理功能
- 内容审核
- 用户管理
- 数据统计
- 系统配置

## 项目结构

```
learning_forum/
├── backend/              # Django 后端
│   ├── config/          # 项目配置
│   ├── apps/            # 应用模块
│   └── requirements/    # 依赖管理
├── frontend/            # Vue 前端
│   ├── src/            
│   │   ├── components/  # 组件
│   │   ├── pages/       # 页面
│   │   ├── stores/      # 状态管理
│   │   └── services/    # API 服务
│   └── public/         # 静态资源
├── docker/              # Docker 配置
├── nginx/               # Nginx 配置
└── docs/                # 项目文档
```

## 开发环境配置

### 后端开发环境
```bash
cd backend
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements/development.txt
python manage.py migrate
python manage.py runserver
```

### 前端开发环境
```bash
cd frontend
npm install
npm run dev
```

### 数据库配置
```bash
# PostgreSQL 安装和配置
createdb learning_forum
psql learning_forum
```

## API 文档

后端 API 文档将通过 Django REST Framework 自动生成，访问 `/api/docs/` 查看完整的 API 接口文档。

## 部署

项目支持 Docker 容器化部署，详细部署说明请参考 `docs/deployment.md`。

## 贡献指南

1. Fork 项目
2. 创建功能分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

## 许可证

本项目采用 MIT 许可证 - 查看 [LICENSE](LICENSE) 文件了解详情。

## 联系我们

- 项目仓库: [GitHub](https://github.com/Feipi/LearnHub)
- 问题反馈: [Issues](https://github.com/Feipi/LearnHub/issues)
- 邮件联系: 3068315381@qq.com
