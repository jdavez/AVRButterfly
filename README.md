### Programming Application Through Bootloader

Connect the serial port (RS232) to J406 3-pin UART.
Press the joystick center button and run
```
avrdude -p atmega169 -P /dev/ttyS1 -c butterfly -U flash:w:main.hex
```


### Programming the Bootloader
Using AVR ISP, connect the 6-pin header to J403 ISP, run
```
avrdude -p atmega169 -P /dev/ttyS1 -c avrispv2   -U flash:w:butterfly_boot_rev04.hex
```
