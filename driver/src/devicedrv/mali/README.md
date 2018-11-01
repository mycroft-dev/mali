# Mali module build instructions for the Mycroft MK2

```
export ARCH=arm64 CROSS_COMPILE=aarch64-linux-gnu-
cd driver/src/devicedrv/mali
KDIR=/path/to/kernel-source BUILD=release MALI_PLATFORM="arm" USING_DT=1 MALI_SHARED_INTERRUPTS=1 MALI_QUIET=1 make
```

Reverse engineered from https://github.com/Xilinx/meta-xilinx/blob/rel-v2018.2/meta-xilinx-bsp/recipes-graphics/mali/kernel-module-mali.bb
