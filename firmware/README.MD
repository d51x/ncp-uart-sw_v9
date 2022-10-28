NCP Firmware for EFR32MG1B / EFR32MG1P

EmberZnet v.7.1.0

ezsp v9

TX - PA0

RX - PA1


Bootloader GPIO Actiovation PD15 low level




bootloader_legacy.* is a original bootloader __EFR32 Serial Btl v6.2.1.3 b0__

прошить можно только через ST-Link / J-Link

eblink.exe -I stlink,dr -S silabs-auto -P /scripts/ -F verify,run,file=bootloader_legacy.hex

