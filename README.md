# Miku UI GSI

**中文** | [English](README-EN.md) | [日本語](README-JP.md)

## 前言
这是送给所有Miku粉丝的Android项目，如果不喜欢它请关闭本页面，但不要攻击任何人，尤其是其作者。

## 版本
最新版本: 0.12.0

[下载](https://github.com/xiaoleGun/treble_build_miku/releases)

## 变体
示例
> MikuUI-TDA-0.13.3-arm64-ab-vndklite-gapps-20230406-UNOFFICIAL.img.xz

从前到后，分别为
```
ProjectName-{SNOW | SNOWLAND | TDA | Udon}-版本号-arm64-ab-vndklite-gapps-构建日期-构建类型
 |                |          |     |               |    |     |      |
 |                |          |     |               |    |     |      |
 |                |          |     |               |    |     |   谷歌服务
 |                |          |     |               |    |     |
 |                |          |     |               |    |     |
 |                |          |     |               |    |    用于vndklite的设备
 |                |          |     |               |    |    支持system读写
 |                |          |     |               |    |
 |                |          |     |               |  分区类型，仅构建AB(1)
 |                |          |     |               |
 |                |          |     |               |
 |                |          |     |          CPU架构，构建64位和a64(2)
 |                |          |     |
 |     Android 12 | 12.1     | 13  | 14
 |
Miku UI
```

(1) 安卓9及以上的底包支持SAR(system-as-root)，所以可以使用AB分区类型的GSI

(2) arm32 binder64

## 构建
要开始构建Miku UI GSI，您需要熟悉[Git和Repo](https://source.android.com/source/using-repo.html)和[How to build a GSI](https://github.com/phhusson/treble_experimentations/wiki/How-to-build-a-GSI%3F).
- 安装依赖
    ```
    sudo apt-get install bc bison build-essential ccache curl flex g++-multilib gcc-multilib git gnupg gperf imagemagick lib32ncurses5-dev lib32readline-dev lib32z1-dev liblz4-tool libncurses5 libncurses5-dev libsdl1.2-dev libssl-dev libxml2 libxml2-utils lzop pngcrush rsync schedtool squashfs-tools xsltproc zip zlib1g-dev xattr openjdk-11-jdk jq android-sdk-libsparse-utils python3 python2 repo
    ```
- 新建Miku工作区并进入
    ```
    mkdir miku-treble && cd miku-treble
    ```
- 下载本仓库
    ```
    git clone https://github.com/xiaoleGun/treble_build_miku -b Udon_v2
    ```
- 完成之后运行脚本:
    ```
    bash treble_build_miku/build.sh
    ```

## 感谢
- [Miku-UI](https://github.com/Miku-UI)
- [phhusson](https://github.com/phhusson)
- [AndyCGYan](https://github.com/AndyCGYan)
- [ponces](https://github.com/ponces)
- [eremitein](https://github.com/eremitein)
- [kdrag0n](https://github.com/kdrag0n)
- [Peter Cai](https://github.com/PeterCxy)
- [haridhayal11](https://github.com/haridhayal11)
- [sooti](https://github.com/sooti)
- [Iceows](https://github.com/Iceows)
