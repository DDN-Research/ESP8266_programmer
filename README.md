# ESP8266_programmer

![6240701_2](https://github.com/DDN-Research/ESP8266_programmer/assets/71212733/abc51c11-0427-4eac-ae4e-6cc6aaa22ef0)

<b>Introduction</b>

<p style="text-align: justify;">Programmer for ESP8266 modules with automatic programming mode.</p>
<p style="text-align: justify;">The need has arisen for small-scale programming of ESP8266 modules. These modules are used in many IoT devices where WiFi communication is required.</p>
<p style="text-align: justify;">Software - programmer was developed. Physical implementation - an ordinary module with a UART-USB converter on board is taken, ESP8266 is removed from it (ESP-1, ESP12E - variants are many), and then 2 ways: putting a special pad for the module (if the module is programmed outside the board), or connecting cable to the module, soldered into the printed board of the product. Usually, these are pins: plus and minus power, EN, RESET, UART_TX, UART_RX, GPIO0. The program itself is written in a Microsoft VisualStudio environment. <p>The software does not require installation and can be launched from any location on the disk.</p>
<p>The developed programmer has a number of features different from others.</p>
<p>1. It can program at a high data transfer rate of 3000000 BAUD. I must immediately note that not all USB-to-UART converters support this speed (see the datasheet of the converter chip). This is not the standard speed of the module. To ensure that work at such a speed, first, before actually filling in the firmware, upload a special program to the module, which allows to work at such a speed of exchange.</p>
<p>2. Mode "Automatic ReStart". This mode allows you to perform small series programming. Before you start working in the program, you set the necessary settings, select the dump file, select this mode and press "Start". The software waits until the module is plugged in, performs firmware flashing of the chip, then waits until the programmed module is unplugged and a new one is plugged in for programming.</p>
<p>Without any operator action other than replacing the module. This significantly reduces the programming time of the modules in series production.</p>
<p>This program is successfully used in production.</p>
<p>P.S. There is a similar program for ESP32 as well, but so far it is only for internal use, passing something like a run-in.</p>
<p></p>
<p>Developer: DDN Research, Ukraine</p>
<p>https://github.com/DDN-Research</p>

<hr>

<b>Manual instruction</b>

<p align=”justify”>
