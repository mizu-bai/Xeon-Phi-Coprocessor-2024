# Xeon-Phi-Coprocessor-2024

Using Xeon Phi Coprocessor in 2024

## Table of Contents

1. Platform
2. Setup

## Platform

|  Components |                Models                |
|:-----------:|:------------------------------------:|
|     CPU     |               E5-2680v4              |
|    Memory   |        DDR4 REG ECC 16 GB * 2        |
| Motherboard |            Huanan X99 CH8            |
|   Storage   | Intel 535s 240 GB + TOSHIBA HDD 1 TB |
|   MIC Card  |            Xeon Phi 3120A            |
|    Power    |           Great Wall 1560W           |

## Setup

The latest MPSS, 3.8.6, can be found here, [Intel Xeon Phi (KNC) MPSS software and kernel modules for CentOS 7&8](https://jjkeijser.github.io/mpss). Since it is not fully compatible with CentOS 8, I decided to switch back to CentOS 7.9. 

Softwares to be installed:

1. MPSS 3.8.6
2. Intel Parallel Studio XE 2017
3. OpenCL Runtime 14.2

### MPSS

**Remember to run `micctrl --initdefaults` before `systemctl start mpss.service`!!!** (Ref: https://community.intel.com/t5/Software-Archive/Xeon-Phi-3120A-boot-aborted-no-configuration-file-present/td-p/1151886)
