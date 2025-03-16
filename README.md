# 立新智能协同云图库项目介绍

项目介绍：基于Vue3+Ant Design+Pinia+AI+WebSocket的企业级智能协同云图库平台。
分为公共图库、私有图库和团队共享图库三大模块。用户可在平台公开上传和检索图片；管理员可以上传、审核和管理分析图片。个人用户可将图片上传至私有空间进行批量管理、多维检索、编辑和分析；企业可开通团队空间并邀请成员，共享和实时协同编辑图片。

主要工作

1.基于Vue3+Ant Design Vue组件库，开发公共图库、私有空间、团队管理、图库分析等15个页面。

2.使用create-vue脚手架+Vite初始化项目，自主开发了包含全局页面布局、导航菜单和通用组件的前端模板，便于后续复用。

3.采用TypeScript+ESLint进行前端工程化管理，并自定义了ESLint规则，提高项目编码质量。

4.全局状态管理：基于Pinia定义UserStore实现了对用户登录态的存储，并通过组合式API(useStore)在各页面中访问用户信息。

5.管理页面：基于Ant Design的Table+Form组件实现了各类管理界面支持分页、筛选、排序、搜索，并利用插槽特性优化了表格列的展示效果。

6.图片搜索：支持关键词、标签分类、颜色搜索、以图搜图等多维度检索，基于ref+watchEffect自动监听搜索条件并发起查询请求。

7.图片优化：采用图片压缩、懒加载、缩略图、CDN加速、浏览器缓存等措施，提升页面加载速度节省流量。

8.实时协作：基于WebSocket事件驱动实现图片协同编辑，通过"编辑锁”与冲突检测机制防止编辑冲突，提升团队协作效率。



![image](https://github.com/user-attachments/assets/379f1ac2-2ef5-4ea5-88ce-efe5e969e8e2)


后端

Java Spring Boot 框架

MySQL 数据库 + MyBatis-Plus 框架 + MyBatis X

Redis 分布式缓存 + Caffeine 本地缓存

Jsoup 数据抓取

COS 对象存储

ShardingSphere 分库分表

Sa-Token 权限控制

DDD 领域驱动设计

WebSocket 双向通信

Disruptor 高性能无锁队列

JUC 并发和异步编程

AI 绘图大模型接入

多种设计模式的运用

多角度项目优化：性能、成本、安全性等

前端

Vue 3 框架

Vite 打包工具

Ant Design Vue 组件库

Axios 请求库

Pinia 全局状态管理

其他组件：数据可视化、图片编辑等

前端工程化：ESLint + Prettier + TypeScript

OpenAPI 前端代码生成
