[![License: LGPL v3](https://img.shields.io/badge/License-LGPL%20v3-blue.svg)](http://www.gnu.org/licenses/lgpl-3.0)

# echo(Distributed IP Proxy System)


Echo是一个分布式的代理共享和管理系统，以长链接的方式连接多个运行在任意位置的终端，并将终端的网络资源整理为一套代理ip集群系统。echo提供整体的鉴权、流量监控、quota控制的功能。

1. Echo天然支持复杂网络环境，所以可以将代理终端部署在手机(甚至树莓派等终端设备)
2. Echo支持代理ip统一的集群管理，所以可以作为ADSL拨号的服务资源的的统一管理出口。使用ADSl使用统一的，稳定的ip出口提供代理服务(而不需要沉重的redis负担)
3. Echo支持sdk，目前提供完善的android APK和gradle依赖(这个作用你懂的😁)
4. Echo分布式设计，天然集群版，无资源瓶颈上限。各节点自动双通道HA热备，无单点风险。
5. Echo全程NIO设计，对资源消耗少，支持并发高(所以代码难度大，可以买个好价钱)，理论上代理最大吞吐占满节点带宽。
6. Echo系统扩展能力强，原则是echo的底层设计使得echo支持任意网络协议转发（udp、tcp、vpn等），且任意协议支持不需要终端升级
7. 终端命令控制，你可以通过http接口将特定指令下发到对应终端.实现如shell执行、ip重播等需求。

# 多平台镜像地址

|平台|地址|备注| 
|--|--|--| 
|github|https://github.com/virjar/echo/|国际|
|gitee|https://gitee.com/virjar/echo|国内|
|virjar|https://git.virjar.com/echo/echo|主地址|

# 多项目友情链接(商务合作+v: virjar1 )

|项目|介绍|地址| 
|--|--|--| 
|echo|分布式代理ip共享集群|https://git.virjar.com/echo/echo|
|sekiro|基于长链接和代码注入的Android private API暴露框架|https://github.com/virjar/sekiro|
|ratel|Android重打包注入引擎|https://git.virjar.com/ratel/ratel-doc|
|zelda|app多开分身的另一种实现|https://github.com/virjar/zelda|
|geeEtacsufbo|极验滑块js代码脱壳-js控制流平坦化反混淆(最早使用AST解除JS流程混淆的项目)|https://github.com/virjar|
|thanos|java爬虫调度系统，让java爬虫重回巅峰！！(开发中)|https://github.com/virjar/thanos|

# 章节目录

1. [软件架构](./doc/1.architecture.md)
2. [快速上手](./doc/2.quick_start.md)
3. [PC客户端部署](./doc/3.jvm_installer.md)
4. [SDK集成](./doc/4.sdk.md)
4. [服务器部署](./doc/5.server_deploy.md)
4. [服务器Docker部署](./doc/5.server_docker_deploy.md)

# echo子项目

## echo网站前端系统

https://github.com/virjar/echo-fe

## echoAndroid客户端

https://github.com/virjar/echo-android

## 请允许我打个广告赚点儿钱

代理云ip推广 [http://i0k.cn/5ewVg](http://i0k.cn/5ewVg)
或扫描下面二维码免费领取ip
![扫码领取ip](doc/img/dailiyun_ad_free_proxy.jpg)

# 社区

加V：（virjar1）,备注echo入群