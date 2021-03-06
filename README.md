# NFramework.TaskHandler
基于消息队列的任务处理框架（待完成）

## 背景

ERP：
* 大数据量
* 批量操作
* 特定组织之间无关联，操作无影响
* 同一组织机构操作需顺序执行，以保证结果的正确性

基于此背景开发此任务处理框架（或者叫消息处理框架）

## 框架时序图

![框架时序图](https://github.com/hzy19860111/NFramework.TaskHandler/blob/master/resource/nframeworksequencediagram.png)

## 架构图

![框架架构图](https://github.com/hzy19860111/NFramework.TaskHandler/blob/master/resource/arch.png)

## 框架特点
* 可水平扩展
* 单队列无并发
* 开发方便，不需要线程知识也能开发多线程处理程序
* 无特定依赖（目前只强依赖log4net，后面解耦）
* 提供Redis队列实现
* 路由机制（可自定义路由规则）


## ToDO
* log4net解耦
* TaskQueueCount、TaskQueueType以及RedisAppName 整合为Setting，每个单独任务 有单独的Setting
* 文档整理
