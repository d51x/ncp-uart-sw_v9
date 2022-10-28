NCP Firmware for EFR32MG1B / EFR32MG1P

EmberZnet v.7.1.0

ezsp v9

TX - PA0

RX - PA1


Bootloader GPIO Actiovation PD15 low level



Ember Standalone Bootloader

bootloader_legacy.* is a original bootloader __EFR32 Serial Btl v6.2.1.3 b0__

прошить можно только через ST-Link / J-Link

eblink.exe -I stlink,dr -S silabs-auto -P /scripts/ -F verify,run,file=bootloader_legacy.hex


Docs:

Ember Standalone Bootloader - https://www.silabs.com/content/usergenerated/asi/cloud/attachments/siliconlabs/en/community/wireless/zigbee-and-thread/forum/jcr:content/content/primary/qna/how_to_realize_theo-j31B/AN760-Using-Standalone-Bootloader.pdf

Gecko Bootloader - https://www.wless.ru/files/Silabs/EFR32/ug266-gecko-bootloader-user-guide.pdf



Скрипты Elelabs (https://github.com/Elelabs/elelabs-zigbee-ezsp-utility), предварительно скачать, например сюда /usr/ota_staging/

cd /usr/ota_staging/elelabs-zigbee-ezsp-utility

python Elelabs_EzspFwUtility.py probe -p /dev/ttyUSB0

![image](https://user-images.githubusercontent.com/10882718/198719216-f3f14694-351c-4679-b59d-e1f0c724fcb8.png)


python Elelabs_EzspFwUtility.py restart -m nrml -p /dev/ttyUSB0

![image](https://user-images.githubusercontent.com/10882718/198719110-ea99b3ac-4a54-45b7-ab11-4450718c6e52.png)


python Elelabs_EzspFwUtility.py restart -m btl -p /dev/ttyUSB0

![image](https://user-images.githubusercontent.com/10882718/198719050-d7779da7-d747-490a-b643-41d6002be01e.png)

