# ModBus-Sniffer
PLEASE NOTE! this is an on goin project and not complete.
Firmware to be used with an ESP to create a bridge between ModBUS RTU and MQTT.
It is meant to be easily configurable for indavidual use cases but will need Devices and Registers setup initually in firmware. It uses the fact that the request and reply use the same first 2 bytes to identify messages. Checksums and time is ignored for simplicity sake. The reply "byte size" is then identified and used to determine regiser size and parsing. A max of 64 bits can be read.
