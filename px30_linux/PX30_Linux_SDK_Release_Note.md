# PX30 Linux SDK Release Note

---

**Versions**

[TOC]

---
## px30_linux_release_v1.4.0_20201203.xml Release Note

**Buildroot (2018.02-rc3)**:

```
- Upgrade chromium to 86.0.4240.111
- Fix RGA blending error when global alpha too large
- qt5multimedia: Fix crash after finished playing
- Update weston to fix some bugs
```

**Debian (buster/10)**:

```
- Upgrade debian9 to debian10
```

**Yocto**:

```
- Upgrade Yocto from 3.0 to 3.2
```

**Kernel (4.4)**:

```
- Fix multivideo and wifi CVE issues
- Fix gsl3673 touch issue on standby
- Fix gcc9 stringop-truncation compilation error
```

**docs/tools**:

```
- windows: RKDevTool: update V2.79 to support new loader format
- linux: package-file: Drop out-dated :grow flag
- Upgrade Linux_Upgrade_Tool to V1.57
- Upgrade DriverAssitant to V5.0
- Update AVL documents
- Update Kernel documents
- Update Linux documents
- Add Benchmark KPI for rockchip linux
```

## px30_linux_release_v1.3.0_20200224.xml Release Note

**kernel**:

```
- fixes the exception that is related with display
- fixes wifi initialization failure
- fixes wifi "pno scan failed"
```

**buildroot**:

```
- fixes wrong capacity for mtp
- use qsetting application instead of old setting applcation
- fix seek video error
- support ums feature
- support webrtc
- support gcc 8.1.0
- add a uvc_app for camera debug test
```

**debian 10**:

```
- aarch64 debian 10 buster release
```

## px30_linux_release_v1.2.2_20191205.xml Release Note

**kernel**:

```
- fixes upgrade issue for nand flash
```

**rkbin**:

```
- ixes IDB backup regions break up the FTL data region
```

**u-boot**:

```
- fixes IDB backup regions break up the FTL data region
```

**camera_engine_rkisp**:

```
- remove dependancy with libdrm that fixes the crash whitout the display system
```

## px30_linux_release_v1.2.1_20191012.xml Release Note

**kernel**:

```
- Fix the low-propability crash whilst high cpu frequency and low ddr frequency at the same time
```

## px30_linux_release_v1.20_20190916.xml  Release Note

**Buildroot(2018.02-rc3)**:

```
- support up to Qt 5.12.2
- support chromium brower
- weston support dual panel same display and dual panel different display
- weston suoport rotate and scale
- support x11 packages
- mali support x11
- provide a mali that has only opencl feature
- add a customized configuration for robot product
- enable ccahe to improve compile speed
- fix compile error on ubuntu 19.04
- support zstd compression algorithm for squashfs
- upgrade glibc to 2.29
```

**kernel**:

```
- upgrade to 4.4.189
- fix logo blink issue
- fix some power regulators can't turn off while suspending
- add a customized configuration for robot product
```

**rkisp upgrade to v2.2.0**:

```
- support blink light control
- optimize capture process
```

**rkbin**:

```
- ddr.bin upgrade to v1.13
- bl32 upgrade to v1.12
    fix ota upgrade failure
- bl31 upgrade to v1.16
    support uart0 wakeup
    support atags
    support boot from secondary cpu
- miniloder upgrade to v1.15
```

**tools**:

```
- Androidtool upgrade to v2.69
```

**applications**:

```
- remove the original gallery,video,music applications, provide the new application to replace
- use the new camera application, that is compatible with the usb camera, and support the differents camera switching
- various fix
```

## rk3326_linux_release_v1.10_20190425.xml Release Note

**Buildroot(2018.02-rc3)**:

```
- WiFi/BT compatibility support
- bluetooth a2dp support
- recovery image size optimization
- support secure boot
- fix sound playback issue for h264
- fix video display issue for h264
```

**document**:

```
- recovery guide
- pcba guide
- hdmi cec guide
- drm display driver development guide
```

**tools**:

```
- DriverAssitant upgrade to v4.8
- AndroidTool upgrade to v2.67
- FactoryTool upgrade to v1.66
- rename rk_provision_tool to RKDevInfoWriteTool, and upgrade to v1.0.4
```

**kernel**:

```
- fix rkisp interrupt storm in some scenarios
- fix kernel lockup after the system is resumed, it's caused by nand/sfc flash
- fix kernel lockup while the watchdog is enable
- memory log (pstore) support
- fix loader upgradation fail upduring ota
- fix powerup failure for ov5695
- add the support for 4k page spi nand flash:ATO25D1GA, XT26G02B, XT26G01B, HYF4GQ4UAACBE
- hardware crypto feature support
```

**Application**:

```
- fix touch event invalid scenario
- improve bluetooth feature
- mpeg4 video support
- fix the hangup after takephotos continuously
- fix the others device can't connect to AP
- wav and wma audio support
```

**rkbin**:

```
- ddr.bin upgrade to v1.11
```

**uboot**:

```
- add the support for NandFlash H27TDG8T2D8R
- support kernel compression image
- add the low voltage protection for PMIC rk809/rk817
- add the watchdog support
- add the MEDIA_BUS_FMT_RGB666_1X7X3_JEIDA format support for lvds display
```

**rkisp**:

```
- upgrade to v2.0.0
```

**libdrm**:

```
- switch branch to rk33/mid/9.0/Develop
```

## rk3326_linux_release_v1.00_20190215.xml Release Note

**buildroot**:

```
- add a simple configuration for robot product
- fixup ssh error on squashfs filesystem
- camera_engine_rkisp upgrade to v1.6
- add camera test scripts
- imporve audio test scripts
```

**rkbin**:

```
- bl32 fix a low probability system hangup
```

**u-boot**:

```
- enable OF_LIVE feature
- add a new configuration without bl32
```

**kernel**:

```
- support black/white camera
- enable rockchip pvtm feature to optimize power consumption
- support camera sensor:ov7750, 0v7251, ov7725
- rk817/rk809 codec support S32_LE
```

**document**:

```
- RKISP_Driver_User_Manual guide
- camera_engine_rkisp_user_manual guide
```