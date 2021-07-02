# jd-base
一键搭建shuye72/jd-base:gitee环境

## 一键运行
```bash
wget -q https://raw.githubusercontent.com/AkaneMurakawa/jd-base/main/jd-base.sh -O jd-bash.sh && chmod +x jd-bash.sh && ./jd-bash.sh
# 测试京东豆变化
# docker exec jd bash jd jd_bean_change now
```
## 小白一键运行
针对小白，可以下载`run_ones.sh`，一键安装Docker和运行jd-base

## Windows开机自动启动虚拟机系统
- 下载脚本[run_virtual_vm_on_windows_started.bat](https://github.com/AkaneMurakawa/my-script/blob/main/run_virtual_vm_on_windows_started.bat)
- 打开为文本，按照脚本的内容进行修改执行


## 控制面板
- 如未修改用户名密码，则初始用户名为：admin，初始密码为：shuye72
- 请访问 http://\<ip\>:5678 登陆并修改配置...
  
## 常见问题
### 运行失败-443... failed: Connection refused
- 使用命令`ll | grep jd-bash.sh`查看`jd-bash.sh`
- 修改hosts
```
vim /etc/hosts
# 增加下面内容
199.232.68.133 raw.githubusercontent.com
  
或者
sudo su;
echo "199.232.68.133 raw.githubusercontent.com" >> /etc/hosts
```
- 若是仍不行，则自行手动下载`jd-bash.sh`
- 手动运行`jd-bash.sh`
  
### 控制面板打开失败  
请确保docker运行的命令和jd-bash.sh是一致的，切勿随便增添参数
  
## 免责声明
- 此仓储脚本仅用于学习研究，不保证其合法性、准确性、有效性，请根据情况自行判断，本人对此不承担任何保证责任。

- 由于此仓储脚本仅用于学习研究，您必须在下载后 24 小时内将所有内容从您的计算机或手机或任何存储设备中完全删除，若违反规定引起任何事件本人对此均不负责。

- 请勿将此仓储脚本用于任何商业或非法目的，若违反规定请自行对此负责。

- 此仓储脚本涉及应用与本人无关，本人对因此引起的任何隐私泄漏或其他后果不承担任何责任。

- 本人对任何脚本引发的问题概不负责，包括但不限于由脚本错误引起的任何损失和损害。

- 如果任何单位或个人认为此仓储脚本可能涉嫌侵犯其权利，应及时通知并提供身份证明，所有权证明，我们将在收到认证文件确认后删除此仓储脚本。

- 所有直接或间接使用、查看此仓储脚本的人均应该仔细阅读此声明。本人保留随时更改或补充此声明的权利。一旦您使用或复制了此仓储脚本，即视为您已接受此免责声明。
