
## 适用场景

将业务应用从自建 Zookeeper 冷迁到 TSE Zookeeper，在迁移过程中，新部署的业务应用不提供服务

## 迁移步骤

### 持久化数据迁移（若有）

将持久化数据迁移到 TSE Zookeeper

### 新部署的业务应用接入

新部署的业务应用接入 TSE Zookeeper，暂时不对外提供服务

### 新部署的业务应用上线

验证新部署的业务应用运行正常

将请求切换到新部署的业务应用

下线存量的业务应用
