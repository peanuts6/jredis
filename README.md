# jredis

## 初步的功能点
* 典型的命令实现(先期考虑用java原生结构)
* 实现连接管理命令      包括 Auth ECHO PING QUIT SELECT 
* 实现发布和订阅命令    包括 publish SUBSCRIBE 等命令
* 实现事务相关命令 包括 watch multi exec 命令实现

## 第一轮迭代周期的内容
* NIO部分 单线程reactor 模型
* 命令分发器
* session 管理 为消息推送，事务提供一些支持
* 简单命令实现（包括字符串，hash，数组）
* 实现连接管理命令
* 实现事务管理命令

## 参考网址
* resp
* https://redis.io/topics/protocol
* 命令参考
* http://doc.redisfans.com/

## 后面的大体计划
* 完全兼容redis命令
* 实现持久化功能
* 合并jcache
* 实现集群功能