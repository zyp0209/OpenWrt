## 说明

- 本项目使用 Github Actions 下载 [Lean](https://github.com/coolsnowwolf/lede) 的 `Openwrt` 源码仓库，进行云编译打包。
- 基于flippy大的打包脚本打包，适配的机型有：`微加云`、`贝壳云`、`我家云`、`N1`、`S905x3`（包括常见的`hk1`、`h96`、`x96`等盒子）、`s922x`（目前支持`GT-King`、`GT-King Pro`两款盒子） 等！
- 本项目使用每周定时编译（北京时间每周六凌晨2点自动触发编译）。
- Releases中的直刷固件分为[➦MINI版](https://github.com/hhaibo/ARMv8-OpenWrt/releases/tag/ARMv8_MINI) 和[➦PLUS版](https://github.com/hhaibo/ARMv8-OpenWrt/releases/tag/ARMv8_PLUS)，MINI版适合科学上网为主要需求的用户，PLUS版是正常多插件版本集成各种常用插件。
- 固件默认IP：`10.10.10.11` 默认密码：`password`
- +的内核版本较新；+o的版本相对+的内核更稳定；f大不太建议N1等盒子使用+的版本，因此比较推荐使用+o的版本。
- 刷机和升级方法以及注意事项请参考f大这两个帖子：[➦旧帖](https://www.right.com.cn/forum/thread-4055451-1-1.html) 和 [➦新帖](https://www.right.com.cn/forum/thread-4076037-1-1.html)
- U盘写入EMMC：登录OpenWrt → 系统 → 晶晨宝盒 → 安装OpenWrt → 选择型号 → 安装
- 升级OpenWrt：登录OpenWrt → 系统 → 晶晨宝盒 → 手动上传更新 → 上传你下载的固件 `或者` 在线下载更新 → 检查固件版本
- 不要盲目追新，仓库自动编译打包的固件插件均为最新的版本，最新版本意味着可能有BUG；如果之前固件使用稳定，无需追新。

## Mini版插件预览
 ![插件预览](https://github.com/hhaibo/ARMv8-OpenWrt/blob/main/imgs/mini.jpg)
 
## Plus版插件预览
 ![插件预览](https://github.com/hhaibo/ARMv8-OpenWrt/blob/main/imgs/plus.jpg)

## 喜欢的可以给个Star，要自己编译独一无二的可以Fork，感谢各位！
本项目使用说明
- 右上角点击自己头像 → Settings → Developer settings → Personal access tokens里面创建个人访问令牌，固件发布会调用，否则无法发布
- Fork本项目
- 点击Actions → 要编译的Workflows → Run workflow → Run workflow 一般一次编译要3~5小时
- `Mini OpenWrt` Mini精简版编译和打包
- `Plus OpenWrt` Plus常用版编译和打包
- `Package` 用编译好的临时固件进行打包，一般是在内核更新需要单独打包的时候运行
- `Make Config` 生成config文件，将自己简单的config文件生成更全面的config文件

## 声明
- 刷机有风险！我只是出于个人爱好学习编译创建的这个项目，刷此固件本人不承担任何后果和技术支持！

## 感谢 ❤️

- [flippy](https://github.com/unifreq/openwrt_packit)
- [ophub](https://github.com/ophub/op)
- [P3TERX](https://github.com/P3TERX/Actions-OpenWrt)
- [breakings](https://github.com/breakings/OpenWrt)
- [mingxiaoyu](https://github.com/mingxiaoyu/N1Openwrt)
- [coolsnowwolf/lede](https://github.com/coolsnowwolf/lede)
