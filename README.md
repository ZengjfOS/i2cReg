# README

## i2c-tools Download

https://mirrors.edge.kernel.org/pub/software/utils/i2c-tools/i2c-tools-4.1.tar.xz

## Android

Android移植参考：[Android.mk](i2c-tools/Android.mk)

## YOCTO

`local.conf`中添加`i2c-tools`即可

## 说明

* 脚本程序：
  * [i2creg for Android](i2creg_Android)
  * [i2creg for Linux](i2creg_Linux)
* 使用说明：
  ```
  ===========================================
  USAGE:
    -h|-?)
    -r)  read all registers
    -w)  write all registers
    -s)  set/get register
    -p)  console print register
    -c)  check chip exist
    -d)  device address
    -b)  read/write all registers begin index
    -e)  read/write all registers end index
    -a)  chip check register address
    -v)  chip check register value
    -f)  read/write data path
    -i)  i2c bus index
  Info:
      current data path: /storage/emulated/0/Music/reg.data
  ===========================================
  ```
