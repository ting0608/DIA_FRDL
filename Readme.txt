1. Copy the partition file included which name as: "cc_frdl"

2. Install ESP board in arduino IDE by adding this into preferences: "https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json"

3. Install ESP ver1.0.4 board

4. Direct to path "C:\*username*\*username*\AppData\Local\Arduino15\packages\esp32\hardware\esp32\1.0.4\tools\partitions" and paste the partition file into it

5. Direct to "C:\*username*\*username*\AppData\Local\Arduino15\packages\esp32\hardware\esp32\1.0.4\boards.txt" and add these line of code:
esp32wrover.menu.PartitionScheme.partitions=cc frdl scheme (3145750 bytes)
esp32wrover.menu.PartitionScheme.partitions.upload.maximum_size=3145750
esp32wrover.menu.PartitionScheme.partitions.build.partitions=cc_frdl

6. Direct to "C:\*username*\*username*\AppData\Roaming\arduino-ide" and delete the whole arduino-ide folder to occur changes

7. Change the credentials to your access point(ap) in code

8. Connect to the same host and you are good to go.