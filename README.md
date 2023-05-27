# Tools_SGIN_X10

![X10 foto](https://github.com/SamuEDL/Tools_SGIN_X10/blob/main/Sgin_X10.JPG?raw=true)


## Features/Caracteristicas:
| Item                      | Description |
|---------------------------|-------------|
| Chipset         | Spreadtrum T618   |
| CPU             | 6x ARM Cortex-A55 @ 1820 MHz / 2x ARM Cortex-A75 @ 2002 Mhz   |
| GPU                    | Mali-G52  |
| Ram   | 6 GB |
| Rom      | 128 GB |
| Screen/Pantalla   | 1920 x 1200 IPS |
| Modem  | 4G (sharkl5pro_modem) |
| Android                    | 11  |
| Kernel                    | 4.14.193 |
| Architecture                    |  Arch64  |
| CodeName Spreadtrum Chipset | ums512_1h10 |
| Connections/Conexiones  | MicroSD, Jack y USB-C (OTG) |
| Camera/Camara        | 8Mpxl (Trasera) y 5Mpxl (Delantera) |
| Connectivity / Conectividad  | Wifi 2,4 Ghz/ 5Ghz / Bluetooth|
| Batery / Batería                  | 7000mAh  |
| Project Treble Support       |  Yes |
| Touch controller  / Controlador Tactil     |  - |
| Power management circuit / Circuito de gestión de energía | bq2560x |
| LCD                  | LCDQC8279-5035  |
| Touch / Panel tactil                   | -  |
| Acelerometter  / Acelerometro             | -  |
| Wifi             | sc2355  |

Firmware Tested
- Teclast M40 Pro M1A2 with the sgin X10 kernel


## Others:

Bootloaders
- Unlock Bootloader (Linux): https://www.hovatek.com/forum/thread-32287.html
- Unlock Bootloader (Windows): https://forum.xda-developers.com/t/alldocube-iplay-40-review-an-all-around-tablet-with-some-minor-compromises.4212541/page-6#post-85850877
- Possible Kernel Source (4.14.133): https://github.com/strongtz/linux-sprd


## FLASH GSI: 

1. adb reboot fastboot <- Reinicia en mod fastbootd desde ANDROID
2. fastboot reboot fastboot <- Reiniciar en modo fastbootd desde BOOTLOADER
3. fastboot delete-logical-partition product_a <- ELIMINA PARTICION PRODUCT
4. fastboot flash --disable-verity --disable-verification system_a imagen.img INSTALA LA ROM GSI
5. fastboot -w <- Eliminar datos de usuario/caché 
