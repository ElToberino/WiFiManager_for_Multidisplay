# WiFiManager for Multidisplay
This is a fork of the development branch of tzapu's [WiFiManager](https://github.com/tzapu/WiFiManager/tree/development) customized for [Tobers Multidisplay](https://github.com/ElToberino/Tobers_Multidisplay). It works with ESP8266 and ESP32.

Most changes I made are visual ones: some new/other css rules and some changes in shown menu items.
Beside that I moved the css and javascript definitions in files on SPIFFS - they had become too large and made the portal unstable. I also added a new public function getStaticMode() returning if the connection has been made with a static IP address.
All changes are marked with the comment ///CHANGE MULTISDISPLAY

As mentioned above, this fork was especially made for my program [Tobers Multidisplay](https://github.com/ElToberino/Tobers_Multidisplay). This program uses WifiManager only for the first connection with a WiFi or if WiFi credentials have been erased by user. On normal startup it is not required to call WifiManager because ESPs store WiFi credentials persistently in flash memory. If you want to try this fork of WiFiManager for your own program, remember that you have to save the main css and javascript files on SPIFFS.<br>
<br>
<p align="center">
    <img src="showcase/captive_portal.jpg" width="700">
</p>
<br>
<br>

**Download and Installation**

Just click on "Clone or Download" -> "Download ZIP" to download the library.
Unpack the library into your Arduino libraries folder.<br>
<br>
<p align="center">
    <img src="showcase/howto.jpg" width="700">
<br><br><br></p>

Successfully compiled with Arduino 1.8.12, 1.8.13 / ESP8266 core for Arduino 2.6.3, 2.7.4 / Arduino core for the ESP32 1.0.4.<br>
For further information ta a look at the original project [WiFiManager](https://github.com/tzapu/WiFiManager/tree/development) .
<br>
<br>
<br>
<b>Thanks a lot</b> to tzapu, tablatronix and all the other contributors for their great work.

