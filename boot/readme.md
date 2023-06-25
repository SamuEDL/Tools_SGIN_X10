| Kernel| Based | Kernel Version | Modded | Tested On Sgin X10 |
| --- | --- | --- | --- | --- |
| boot_a | Stock SGIN X10  | 4.14.193 | No | Yes |
| boot_stock | Stock SGIN X10  | 4.14.193 | No | Yes |
| BootMagiskSginX10 | Stock SGIN X10  | 4.14.193 | Patched Magisk 26.1 | Yes |

**Note:** Here there will only be kernels that are 100% compatible with the SGIN X10

# Install:
**Requirements:**
- Unlock Bootloader

**Instructions:** 
1. Install fastboot tools from google's sdk on your PC
2. Enter fastboot mode
3. Run in command line
```
fastboot flash boot_a boot.img 
fastboot flash boot_b boot.img
fastboot reboot
```

**Note:** Replace boot.img, with the name of the kernel.
