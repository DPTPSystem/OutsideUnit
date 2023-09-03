# OutSide Humidity and temperature sensor unit
* author: DPTP System 2023-09-03.
* components: P16F689, AM2322 or BME280 or BME680 or DHT11
* IDE: MPLAB v8.91

# Projekt info
A projekt teljes részetességével nyilvánosan elérhető. Tételesen a következők:
- Altium projekt
- - Schematic
- - PCB
- - 3D objektum
- - Gerber állomány
- MPLAB projekt
- - Az összes forráskód

# Miért
Egy olyan hőmérséklet és páratartalommérő eszközt akarok fejleszteni, amely viszonylag alacsony költségvetéssel kivitelezhető és emellett
a legminimálisabb komponensekből áll.

# Célok
A cél, hogy egy már elkészült beltéri egységemhez készítsek egy adó egységet, amely 2.4GHz-es rádión tólja be megadott időközönként a 
mért hő és pratartalom adatokat.

# Hardver
Egyszerű és itthon is fellelhető olcsóbb elemekből gondoltam össze rakni egy olyan hardvert, amely kiszolgálja az alapvető igényeket.
Az igények közt a következők voltak fontosak: MCU = SPI, I2C, EEPROM, legalább 1 küsőleg triggerelhető megszakítás, belső órajel, 
minimális IO port. A PIC16F689 pontosan kielégíti ezen igényeket, így ezzel gondoltam a projektet kivitelezni. Az eszköz 2.4GHz-es 
rádión küldözgeti majd az adatokat meghatározott időközönként, amelyet még nem tudok, de 10-15percre gondoltam. Ezen felül AM2322 vagy 
BME280-BME680 szenzorokat szeretnék használni, de nem zárom ki a DHT11 lehetőségét sem. Összesen még 1 gomb, 1 LED és a maradék 
perifériákat is kivezetem, hogy ha esetleg szükség lenne rá, ki lehessen használni. (UART, és 4db PORT)
Az eszköz 5v-os USB adapterről, MicroUSB csatlakozó felületről kapja a táplálást.

# Elméleti működés
Folyamatban...