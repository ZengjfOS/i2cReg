# README

## i2c-tools Download

https://mirrors.edge.kernel.org/pub/software/utils/i2c-tools/i2c-tools-4.1.tar.xz

## Android

Android移植参考：[Android.mk](Android.mk)

## read/write连续地址数据脚本

* 脚本程序：[i2cReg](i2cReg)
* 使用说明：
  ```
  ===========================================
  USAGE:
      1. i2cReg -r: read all reg from device
      2. i2cReg -w: write all reg to device
      3. i2cReg -s: read/write  reg from/to device
  Info:
      current data path: /storage/emulated/0/Music/reg.data
  ===========================================
  ```
* 数据路径：修改[i2cReg](i2cReg)脚本中`dataPath`变量即可调整数据存储位置；
* 其他参数配置，请修改[i2cReg](i2cReg)脚本对应位置：
  ```shell
  # Data settings
  dataPath=/storage/emulated/0/Music/reg.data
  
  # Device settings
  i2cBus=5
  deviceAddress=0x48
  regStart=1
  regEnd=113
  
  # Simulate like linux driver check chip
  checkRegAddress=0x1e
  checkRegValue=0x40
  ```
