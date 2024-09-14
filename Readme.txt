# 用于红米 2A 的 Klipper 固件，带 8821/8811cu 5G 网卡驱动

## 刷机步骤

1.下载 firmware.zip 并解压
2.关机模式下按住音量减键开机进入 fastboot 模式
3.运行一键刷机.bat


默认关闭了红米 2A 自带的 WIFI ，若要启用，执行

```bash
sudo insmod ~/wcn36xx.ko
```

若要开机自启，执行

```bash
sudo cp ~/wcn36xx.ko /lib/modules/6.10.0-msm8916+/kernel/drivers/net/wireless/ath/wcn36xx/
```