# 钱包账户网关提供商

这是一个钱包账户网关提供商项目，主要提供以下功能：

## 功能特性

- 银联支付集成
- 钱包账户管理
- 网关服务提供
- 支付处理
- 账户绑定与验证

## 技术栈

- Java 7
- Spring Framework 4.3.3
- Dubbo 2.5.3
- MySQL 5.1
- SQL Server
- Redis
- UnionPay SDK

## 项目结构

```
cz-wallet-account-gateway-provider/
├── src/                    # 源代码目录
├── lib/                    # 依赖库
├── cz-wallet-account-gateway-provider-config/  # 配置文件
├── .project               # Eclipse项目文件
├── .classpath             # Eclipse类路径配置
└── qodana.yaml            # Qodana代码质量检查配置
```

## 配置说明

### 主要配置文件

1. `config.properties` - 主要业务配置
2. `jdbc.properties` - 数据库连接配置
3. `log4j.properties` - 日志配置
4. `acp_sdk.properties` - 银联SDK配置
5. `cz-wallet-account-gateway-provider.xml` - Spring配置

### 数据库配置

项目支持MySQL和SQL Server数据库，通过jdbc.properties进行配置。

## 部署说明

1. 配置数据库连接
2. 配置银联商户信息
3. 配置Redis连接
4. 启动Dubbo服务

## 注意事项

- 请确保所有敏感信息（如数据库密码、API密钥等）在生产环境中正确配置
- 定期检查并更新依赖库版本
- 遵循安全最佳实践进行部署