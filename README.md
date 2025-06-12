## Instructions


1. Project -> esp32-wifi-pentration : https://github.com/risinek/esp32-wifi-penetration-tool

    - step-1: cd into projects/wifi-penetration-tool

    - step-2: ```pip install esptool``` 

    - step-3: run this command (Here COM6 port that esp32 is connected)
        
        ```
        esptool -p COM6 -b 115200 --after hard_reset write_flash --flash_mode dio --flash_freq 40m --flash_size detect 0x8000 partition-table.bin 0x1000 bootloader.bin 0x10000 esp32-wifi-penetration-tool.bin
        ```
