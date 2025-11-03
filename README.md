# LoRa_Atmega328p_window_Door_Sensor
This repository contains the files to create the ATMEGA 328p wireles transmitter using the LoRa RX/TX chip Wio-E5.
![PCB image](https://github.com/gadjet/Lora_Atmega328p_window_Door_Sensor/blob/main/20250926_204523%20-%20Copy.jpg)

The design uses the reed switch wakeup circuit from the earlier ESP-NOW ESP8266 based Window/Door sensor but is now controls the power supply to an ATMEGA 328p device which is then linked via the serial port to a Wio-E5 TX/RX LoRa chip from Seeedstudio.

Much the same as the WiFi based sensor this board is used to detect the status of a window or door but instead of WiFi this sensor uses 868Mhz (915MHz in other countries) to transmit the data over a much greater distance than the WiFi version.

There is also an ISP connector to allow the bootloader to be flashed into the chip but in this first version there was an error on my PCB and one of the connections was left off from the ISP connector and it requires a wire to be added to the PCB to allow flashing of the bootloader (see image).



