<p align="center"><img width="320" src="	
https://cdn.max-c.com/wiki/671860/Download.png?v=1" /></p>
<h1 align="center">
  BattleBit EAC Fix</h1>
  

<a href="https://livingflore.me/eacfix" target="-blank" title="Download">
    <img src="[	
https://cdn.max-c.com/wiki/671860/Download.png?v=1]">
</a>



###<h4>此批处理脚本完全重新安装 EAC，并安装 VCRedist x86-64 2015-2022 以解决此问题和其他问题。


<h2 align="center">
  Further Troubleshooting</h2>

### [•](https://i.imgur.com/tKGFam6.png) 确保您已安装 易反作弊 并使用它运行游戏。
1) 运行批处理（上面的下载按钮）。
2) 确保**两个** VCRedists都安装正确 - [x86](https://aka.ms/vs/17/release/vc_redist.x86.exe) and [x64](https://aka.ms/vs/17/release/vc_redist.x64.exe).
运行安装程序时，您应该能看到 3 个选项：修复、卸载和取消。如果看不到它选择：**继续安装**。
3) 尝试从位于已安装文件中的管理员运行BattlebitEAC.exe或EasyAntiCheat.exe（**右键单击游戏>属性>已安装的文件>浏览**）
4) 您可能会遇到一些连接问题，因此 EAC 无法访问其服务器。尝试使用[Cloudflare WARP](https://1.1.1.1)或任何代理。

### [•](https://i.imgur.com/ADtyLmM.png) 启动错误 - 未安装EAC反作弊。
运行["Install & Repair Easy Anti Cheat"](https://i.imgur.com/466AXn8.png)启动选项。

如果无法访问启动选项，请[右键单击游戏>“属性”>“启动选项”>“启动游戏时询问”](https://i.imgur.com/16aeGuw.png) 

### [•](https://i.imgur.com/yzxejzh.png) 创建文件失败，错误代码32。
1) 重新启动您的电脑。
2) 删除位于 `EasyAntiCheat_EOS.sys` 中的文件。`C:\Program Files (x86)\EasyAntiCheat_EOS`.
3) 运行bat文件（上面的下载按钮）。

### [•](https://i.imgur.com/tDRxBLb.png) 不受信任的系统文件
根据导致此问题的驱动程序，您可能需要[重新安装](https://support.nzxt.com/hc/en-us/articles/4403882406555-Reinstalling-Graphic-Drivers)/更新 GPU 驱动程序

更新 GPU 驱动程序或以管理员身份运行并在命令提示符下（按 Win+R，键入 ，然后按 Ctrl+Shift+Enter）。

### [•](https://i.imgur.com/buVpgid.jpg) 检测到游戏违规
如果看到错误代码#0000000D请删除干扰 EAC 的进程（方括号中的名称）。
对于任何其他错误代码，修复是通用的：

0) 检查您的任务管理器并摆脱您认为会干扰EAC的任何软件（RGB、托盘最小化器、调整等）。
1) 如果使用第三方防病毒软件 - 请确保将EAC添加到排除项。如果它没有帮助 - 关闭这个防病毒软件。
2) 运行bat文件（上面的下载按钮）。
3) 尝试以管理员身份运行BattlebitEAC.exe或EasyAntiCheat.exe（右键单击可执行文件>以管理员身份运行）位于已安装文件中（右键单击游戏>属性>已安装的文件>浏览）。
4) 验证游戏文件。
5) 启用[数据执行保护](https://support.microsoft.com/en-us/topic/what-is-data-execution-prevention-dep-60dabc2b-90db-45fc-9b18-512419135817).
6) 按 Win+R，键入**sigverif**并按回车键。继续进行驱动程序签名验证。完成后，系统将提示您未签名的驱动程序列表或消息，说明一切正常。在第一种情况下，根据未签名的驱动程序，您可能需要[重新安装](https://support.nzxt.com/hc/en-us/articles/4403882406555-Reinstalling-Graphic-Drivers)/更新 GPU 驱动程序
或以管理员身份运行并在命令提示符下（按 Win+R，键入，然后按 Ctrl+Shift+Enter）。

### [•](https://i.imgur.com/mePC8z1.png) 启动服务失败EasyAntiCheat_EOSSys，错误代码5。
1) 运行bat文件（上面的下载按钮）。
2) 按 Win+R，键入**regedit.exe**，然后转到**HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Services\EasyAntiCheat_EOS**，右键单击**EasyAntiCheat_EOS**，并授予对所有应用程序包的完全访问权限。

### [•](https://i.imgur.com/rR0rDnB.png) 你被反作弊踢了。确保...
0) 如果您使用自定义 lang 文件 - 删除它，你没有被封禁。
1) 确保您没有 EAC 条目 `/etc/hosts` (例如，《星际公民》需要这样做)。
2) 运行bat文件（上面的下载按钮）。
3) 确保**绝对没有任何东西** 阻止 EAC 连接（杀毒软件 / 防火墙 / ISP）。
4) 删除 `Certificates` 它位于 [已安装文件](https://i.imgur.com/t8Pocyo.png) > `EasyAntiCheat` 并且 
[验证游戏完整性](https://cdn.discordapp.com/attachments/1109901924314140732/1124030888276132000/BBR_Validation.gif). 
1) 通过重新启动调制解调器/路由器或使加速器/[Cloudflare WARP](https://1.1.1.1).来改变你的IP。
2) 如果以上任何内容都无济于事 - 对不起，您只能靠自己。

### [•](https://i.imgur.com/N8Zyr47.jpg) 应用程序无法正确启动（0xc0000005)
此错误代码表示访问冲突 => 可以是任何东西。
1) 此错误代码表示访问冲突 => 可以是任何东西。
2) 尝试以管理员身份运行BattlebitEAC.exe或EasyAntiCheat.exe([右键可执行文件>以管理员身份运行](https://i.imgur.com/l4kF2o3.png))位于路径下的该文件。([右键游戏>属性](https://i.imgur.com/16aeGuw.png) [>已安装文件>浏览](https://i.imgur.com/t8Pocyo.png)).
3) 按下Win+R键入`cmd`, 然后按下Ctrl+Shift+Enter并运行`sfc /scannow` (可能会花上一段时间) 和 `dism /online /cleanup-image /restorehealth`.
4) 禁用超频软件（如果有）。
5) [验证游戏文件完整性](https://cdn.discordapp.com/attachments/1109901924314140732/1124030888276132000/BBR_Validation.gif).
6) 在其他驱动器/分区上重新安装游戏。

### • 我在上面找不到我的问题...
请联系BattleBit不同社区服务器中的[#anti-cheat-help(DC社区)](https://discord.com/channels/303681520202285057/1023557300214050968)（上面的按钮）尋寻求帮助。
