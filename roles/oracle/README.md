# Description
```
oracle
    ├── defaults
    │   └── main.yml
    ├── handlers
    │   └── main.yml
    ├── tasks
    │   ├── main.yml
    │   ├── install.yml
    │   ├── configuration.yml
    ├── templates
    │   ├── oracle-19c.j2
    │   ├── oracle-19c.conf.j2
    └── vars
    │   └── main.yml
    └── README.md
```
The playbook aims for installing oracle automatically.

You can modify the config documents `/roles/oracle/defaults/main.yml` to customise the parameters about oracle database parameters, for example, oracle-installation-directory and oracle-sid etc.

# Usage
Please satisfy the following conditions, before you enter the command below:
- [x] Ensuring your Linux have installed **Ansible**.
- [x] Modify `host.host` to your expected hosts.
- [x] Modify `roles_list.yml` to your expected software installation.
- [x] Define the configuration you want to modify on the `defaults` directory.

# Version
`v1.0 2020.04.16` Supporting oracle 19c installation

# 说明
```
oracle
    ├── defaults
    │   └── main.yml
    ├── handlers
    │   └── main.yml
    ├── tasks
    │   ├── main.yml
    │   ├── install.yml
    │   ├── configuration.yml
    ├── templates
    │   ├── oracle-19c.j2
    │   ├── oracle-19c.conf.j2
    └── vars
    │   └── main.yml
    └── README.md
```

该playbook旨在安装自动化安装oracle。

你可以通过修改 `/roles/oracle/defaults/main.yml` 的内容来自定义数据库配置，例如，数据库安装路径、数据库实例名等

# 使用方法
在输入下列命令之前，需要确保满足下列条件：
- [x] 确保你的Linux机器已安装了Ansible。
- [x] 将`host.host`配置文件的内容修改为你想要安装的服务器信息。
- [x] 将`roles_list.yml`配置文件的内容修改为你想要安装的软件。
- [x] 修改`defaults`中的变量值，支持自定义路径等配置。

```
ansible-playbook -i host.host roles_list.yml
```

# 版本发布
`v1.0 2020.04.16` 支持oracle 19c安装