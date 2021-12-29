# openwrt_nezha

哪吒监控 For OpenWRT

**暂时仅支持lua版本**



## 简介

用于在旧版OpenWRT及LEDE中快捷添加Nezha客户端的项目，解决OpenWRT需要手动添加服务的问题。



## 用法

### 编译

将 `src-git nezha https://github.com/Erope/openwrt_nezha` 添加至 `feeds.conf.default` 后执行

./scripts/feeds update -a && ./scripts/feeds install -a

找到luci-app-nezha 选中后编译即可



## 安装IPK包

从Release中下载适合的包后自行安装(仅支持X64 X86和ARM64)



## 致谢

部分代码来自P3TERX <https://p3terx.com> 和 KFERMercer <KFER.Mercer@gmail.com>

源项目为: <https://github.com/naiba/nezha>

非常感谢！



## Q/A

1. Q: 我的架构并非X64 X86和ARM64 可以安装吗？

   A: 可以，请自行编译，但需要注意如果性能较弱或者内存过少，启动Nezha可能会严重消耗性能。

2. Q: 我想将其部署在工作压力较大的OpenWRT上，有什么需要注意的吗？

   A: 需要注意Nezha默认会监控连接数，在连接数较多的情况下可能会影响性能。

3. Q: Agent会自动更新吗？

   A: 会自动更新，因此未扩容的硬路由需要注意剩余空间是否足够。

4. Q: 我想更新Agent需要做什么吗？

   A: 一般情况下Agent会自动更新，但本项目的版本号不会自动更新，虽然安装包会跟随Nezha源项目而更新。如若Agent有特殊情况长期未能正常更新，可以考虑删除包后重新安装。

