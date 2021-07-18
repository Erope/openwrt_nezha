# luci-app-nezha-agent
本插件为[nezha-agent](https://github.com/liuzhuoling2011/nezha-agent)的LuCI配置页面, 用于启动以及配置nezha-agent. 

部分代码来自[[CTCGFW]](https://github.com/project-openwrt/nezha-agent/tree/master/luci-app-nezha-agent).

此插件依赖nezha-agent软件包, 你可以在[此处](https://github.com/KFERMercer/openwrt-nezha-agent)找到.

## 如何添加插件 

首先, cd 进你本地的 OpenWrt 项目根目录下, 然后依次执行以下命令: 

`git clone https://github.com/KFERMercer/openwrt-nezha-agent.git ./package/nezha-agent`

`git clone https://github.com/KFERMercer/luci-app-nezha-agent.git ./package/luci-app-nezha-agent`

`rm -rf ./tmp/`

`make menuconfig`

在编译配置菜单中选择`luci-app-nezha-agent`. 
