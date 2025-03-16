# lixin-yun-picture

## 项目介绍
基于 Vue3 + Ant Design + Pinia + AI + WebSocket 构建的企业级智能协同云图库平台，包含三大核心模块：

- **公共图库**：支持用户公开上传和检索图片，管理员可进行图片审核与数据分析
- **私有图库**：个人用户专属空间，提供图片批量管理、多维检索、智能编辑与分析功能
- **团队共享图库**：企业团队协作空间，支持成员实时协同编辑与文件共享

## 主要功能实现
### 前端核心功能
1. **基础架构**
   - 基于 `create-vue` 脚手架 + Vite 初始化项目
   - 自主开发前端模板（全局布局/导航菜单/通用组件）
   - 采用 TypeScript + ESLint（自定义规则）实现工程化管理

2. **功能模块**
   - 开发 15+ 功能页面（公共图库/私有空间/团队管理等）
   - 全局状态管理：基于 Pinia 的 UserStore + 组合式 API 管理登录态
   - 管理界面：Ant Design Table+Form 实现分页/筛选/搜索功能
   - 图片搜索：支持关键词/标签/颜色/以图搜图等多维度检索（watchEffect 监听）

3. **性能优化**
   - 图片优化：压缩/懒加载/CDN/浏览器缓存
   - 实时协作：WebSocket + 编辑锁 + 冲突检测机制

### 后端技术亮点
⭐️ **核心架构**
- DDD 领域驱动设计
- ShardingSphere 分库分表
- Sa-Token 权限控制
- Disruptor 无锁队列

⭐️ **关键技术**
- WebSocket 双向通信
- JUC 并发编程
- COS 对象存储
- AI 大模型接入

⭐️ **系统优化**
- 多级缓存（Redis + Caffeine）
- 安全防护（XSS/CSRF 防御）
- 设计模式实践（工厂/策略/观察者）

## 技术选型
### 后端技术栈
| 类别                | 技术选型                                                                 |
|---------------------|--------------------------------------------------------------------------|
| 基础框架            | Spring Boot 3.x                                                         |
| 数据存储            | MySQL 8 + MyBatis-Plus + MyBatis X                                      |
| 缓存系统            | Redis 7 + Caffeine 3.x                                                  |
| 通信协议            | WebSocket + HTTP/2                                                      |
| 安全控制            | Sa-Token + JWT + Spring Security                                        |
| 数据处理            | ShardingSphere 5.x + EasyExcel                                          |
| 智能处理            | 文心ERNIE 3.0 / Stable Diffusion 模型                                   |

### 前端技术栈
| 类别                | 技术选型                                                                 |
|---------------------|--------------------------------------------------------------------------|
| 核心框架            | Vue 3 + Composition API                                                 |
| UI 组件库           | Ant Design Vue 3.x                                                      |
| 状态管理            | Pinia 2.x                                                               |
| 工程化              | Vite 4 + ESLint + Prettier + OpenAPI 代码生成                           |
| 辅助工具            | Axios + WebSocket-Client + lodash-es                                    |
| 可视化              | ECharts 5 + @antv/g2                                                    |

