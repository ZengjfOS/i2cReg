# README

## i2c-tools Download

https://mirrors.edge.kernel.org/pub/software/utils/i2c-tools/i2c-tools-4.1.tar.xz

## Android

Android移植参考：[Android.mk](Android.mk)

## read/write连续地址数据脚本

* 脚本程序：[i2creg](i2creg)
* 使用说明：
  ```
  ===========================================
  USAGE:
    -h|-?)
    -r)  read all register
    -w)  write alle register
    -s)  set/get register
    -p)  console print register
    -d)  device address
    -b)  register begin index
    -e)  register end index
    -c)  chip check register address
    -v)  chip check register value
    -f)  read/write data path
  Info:
      current data path: /storage/emulated/0/Music/reg.data
  ===========================================
  ```
* 数据路径：修改[i2creg](i2creg)脚本中`dataPath`变量即可调整数据存储位置；
