# Asrock Z370 Taichi & Fatal1ty Z370 Professional Gaming i7 with QTJ1-Hackintosh-Sonoma-OpenCore

本套EFI可以保证启动并且适应macOS Sonoma系统，并且除了不工作的硬件之外没有太大毛病

## 配置信息（这是本人配置，仅供参考）

| CPU    | Intel QTJ1 ES                       |
|:------:|:----------------------------------------:|
| 显卡   | RX580                                    |
| RAM    | 32GB DDR4                                 |
| 声卡     | ALC1220                                   |
| 硬盘     | PM9A1                       |
| 网卡&蓝牙  | Intel AX200           |

## 正常工作

1. CPU变频（其他CPU型号使用[one-key-cpufriend](https://github.com/stevezhengshiqi/one-key-cpufriend)生成对应的kext）

2. 声音正常

3. 麦克风

4. HiDPI，使用一键[HiDPI](https://github.com/xzhih/one-key-hidpi)脚本。

5. WiFI

6. 蓝牙 


## 不工作&小毛病

1. 核显休眠(魔改U禁用ME导致的)

2. 如果您的主板是Fatal1ty Z370 Professional Gaming i7的话需要额外补充Marvell Aquantia AQC107网卡的kext才能让内置的万兆网卡工作

## Q&A

Q1:为啥这个EFI同时兼容Z370 Taichi和Fatal1ty Z370 Professional Gaming i7？ 

A1:因为这两块主板为互相套娃关系，后者比前者主要是多了Marvell Aquantia AQC107万兆网卡。
