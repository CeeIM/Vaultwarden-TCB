<p align="center">
  <img height="100px" src="./logo.png" center />
</p>

# [Vaultwarden-TCB](https://github.com/CeeIM/Vaultwarden-TCB)

在腾讯云开发 Tencent CloudBase 上部署 Vaultwarden (Bitwarden)

## 部署

本项目基于 [腾讯云开发框架](https://github.com/Tencent/cloudbase-framework) + [Vaultwarden](https://github.com/dani-garcia/vaultwarden) 支持一键云端部署

MySQL 部署（MySQL + 文件存储）[![](https://main.qcloudimg.com/raw/67f5a389f1ac6f3b4d04c7256438e44f.svg)](https://console.cloud.tencent.com/tcb/env/index?action=CreateAndDeployCloudBaseProject&tdl_anchor=github&tdl_site=0&appUrl=https://github.com/CeeIM/Vaultwarden-TCB)

SQLite 部署（文件存储）[![](https://main.qcloudimg.com/raw/67f5a389f1ac6f3b4d04c7256438e44f.svg)](https://console.cloud.tencent.com/tcb/env/index?action=CreateAndDeployCloudBaseProject&appUrl=https://github.com/CeeIM/Vaultwarden-TCB&branch=cfs-only)

### 配置

- SIGNUPS_ALLOWED： 是否允许注册

更多配置参考：https://github.com/dani-garcia/vaultwarden/wiki

### 依赖

- CFS：需要使用 CFS 持久化配置数据

## 注意事项

1. 部署时，需要将服务路径设置为根路径 `/`
2. Vaultwarden 默认使用 SQLite 做存储数据库
3. 初始化完成后，请关闭 SIGNUPS_ALLOWED 配置
