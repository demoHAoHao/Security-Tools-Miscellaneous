🛠 工具介绍：Impacket 0.9.23
📌 简介
Impacket 是由 SecureAuth 开发并维护的一套 Python 网络协议工具包，专门用于处理低层级的网络协议交互。它支持多种协议的构造、发送、接收和解析，是渗透测试、红队、内网横向移动等任务中的核心工具之一。

当前版本：impacket 0.9.23

🎯 功能用途
Impacket 提供了多种实用工具，可用于：

SMB 共享枚举与文件操作

NTLM/NTLMv2 抓取与中继攻击

Kerberos 协议攻击（AS-REP Roasting, Ticket extraction 等）

执行远程命令（如通过 psexec, wmiexec, smbexec 等）

内网横向移动

LSA Secrets / SAM / NTDS.dit 提取

DCSync 模拟

🧩 主要模块与脚本
安装后，impacket 会附带多个命令行脚本（一般安装路径 /usr/local/bin/ 或虚拟环境中）：


# 脚本名称	简要说明
{psexec.py	通过 SMB 利用服务安装执行命令（远程执行，类 Meterpreter）
wmiexec.py	利用 WMI 协议远程执行命令（静默执行）
smbexec.py	利用 SMB 管道执行命令并获取输出
secretsdump.py	导出 LSA secrets, SAM hash, NTDS.dit 内容
lookupsid.py	枚举远程主机/域内 SID 到用户名
GetUserSPNs.py	Kerberoasting 攻击工具，列出带 SPN 的用户
GetNPUsers.py	AS-REP Roasting 工具
dcomexec.py	使用 DCOM（如 MMC）远程执行命令
addcomputer.py	添加计算机账户到域
ticketconverter.py	将 kirbi 票据与 ccache 互相转换
ticketer.py	创建自定义 Kerberos TGT（金票）}
--------------------------------------------------------------------------------------
