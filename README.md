# go-version-fetcher

本项目是一个用于自动化安装和管理 Go 语言版本的 Ansible 脚本。通过这个脚本，您可以轻松地在目标主机上安装 Go、设置环境变量以及更新旧版本。

## 特性

- 自动下载和安装指定版本的 Go 语言
- 自动设置 Go 相关的环境变量
- 保留最新的 5 个 Go 版本，同时删除较旧版本
- 自动创建 `/etc/profile.d/go.sh` 文件以设置环境变量
- 
## 注意事项

 - 在运行脚本之前已正确配置 Ansible 环境和目标主机。
 - 仔细检查脚本和变量，以确保其符合您的具体需求。
 - 
## 使用方法

1. 根据您的需求修改 `ansible-playbook` 脚本，配置目标主机等信息。
2. 运行以下命令执行脚本：

```bash
ansible-playbook -i inventory.ini playbook.yaml



