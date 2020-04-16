# Description
This repo aims for installing various software automatically by **Ansible**. 
I will provide the stable (already tested) **playbook** on the below content. 
If that is what you want or make some benefits for you, please click the right side button **【★Star】**.
If there are any problems you found, you can give me an issue, and I will fix it as fast as I can. 
Thanks a lot!
XD

# Contents
roles
    └── oracle

# Usage
Please satisfy the following conditions or you can configure on your own, accroding to the exclusive `README.md` in the every different playbook before you enter the command below:
- [x] Ensuring your Linux have installed **Ansible**.
- [x] Modify `host.host` to your expected hosts.
- [x] Modify `roles_list.yml` to your expected software installation.
- [x] Define the configuration you want to modify on the `defaults` directory.

```
ansible-playbook -i host.host roles_list.yml
```

---

# 说明
该库旨在使用Ansible的playbook脚本来安装各种各样常用的软件，我会不定期上传我编写及使用过的playbook，大家可以通过下面的目录知晓目前已有的playbook，如果发现任何bug，麻烦请给我提交issues，我会尽可能快的解决，如果觉得有帮助的话，请不要吝惜你宝贵的【★Star】，谢谢！

# 目录
roles
    └── oracle

# 使用方法
在输入下列命令之前，需要确保满足下列条件，每个playbook都有对应详细的`README.md`,读者也可根据playbook中的`README.md`来进行修改
- [x] 确保你的Linux机器已安装了Ansible。
- [x] 将`host.host`配置文件的内容修改为你想要安装的服务器信息。
- [x] 将`roles_list.yml`配置文件的内容修改为你想要安装的软件。
- [x] 修改`defaults`中的变量值，支持自定义路径等配置。

```
ansible-playbook -i host.host roles_list.yml
```