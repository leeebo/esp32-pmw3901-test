## 接线


| 名称         | 引脚 |
| ------------ | ---- |
| SPI_SCK_PIN  | 14   |
| SPI_MISO_PIN | 12   |
| SPI_MOSI_PIN | 13   |
| SPI_CS_PIN   | 15   |


## 注意事项

1. 在烧写程序，和启动时，请拔掉GPIO12（MISO），否则flash电压会被配置成1.8v无法进行下一步
2. 或者使用`espefuse.py --port /dev/ttyUSB0 set_flash_voltage 3.3V` 固定flash的电压，进而将gpio12的切换去使能