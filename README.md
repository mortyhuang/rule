# Clash 规则配置

这个仓库包含用于 Clash 的自定义规则配置，配合 [ACL4SSR 在线订阅转换工具](https://acl4ssr-sub.github.io/) 使用。

## 使用方法

1. 访问 [ACL4SSR 在线订阅转换工具](https://acl4ssr-sub.github.io/)
2. 输入你的订阅链接
3. 选择 "Clash" 作为目标格式
4. 在"远程配置"字段中，输入本仓库配置文件的 URL:
   ```
   https://raw.githubusercontent.com/mortyhuang/rule/refs/heads/main/leepooool.ini
   ```
5. 根据需要配置其他选项（emoji、排序等）
6. 点击"生成配置"

## 也可以根据下面这个示例导入

```
http://localhost:25500/sub?target=clash&url=https%3A%2F%2F114.66.57.89%3A21000%2Fce9813bbd909c40265845fadb7e5fb48%7Chttps%3A%2F%2Fwww12.bigairport-eleventh-sub.com%2Fapi%2Fv1%2Fclient%2Fsubscribe%3Ftoken%3D7480779ff1f09902647d31a86382f23b&insert=false&config=https%3A%2F%2Fraw.githubusercontent.com%2Fmortyhuang%2Frule%2Frefs%2Fheads%2Fmain%2Fleepooool.ini&emoji=true&list=false&tfo=false&scv=true&fdn=false&expand=true&sort=false&new_name=true
```
> 第一个订阅链接为主力节点
> 第二个订阅链接为廉价节点


## 配置文件说明

主配置文件 `leepooool.ini` 包含：

- 各种应用和服务的规则集
- 不同地区的代理组
- 自动节点选择的 URL 测试配置
- 广告拦截和隐私保护规则

## 自定义列表

仓库还包含特定服务的自定义域名列表：

- `Emby.list`: Emby 媒体服务器规则
- `F1.list`: F1 相关域名规则
- `Proxy.list`: 需要代理的额外域名
- `Domestic.list`: 直接访问的国内域名
