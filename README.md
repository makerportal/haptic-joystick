# haptic-joystick
Haptic joystick buzzer with Arduino - creating different buzz patterns for different joystick movements with ESP32 arduino board

Get an Analog Joystick module here: [Analog Joystick Module](https://makersportal.com/shop/mini-gps-module-atgm336h-antenna) <br>
See full tutorial here: [Haptic Feedback Joystick with Arduino](https://makersportal.com/blog/haptic-feedback-joystick-with-arduino) <br>

# 
### JUMP TO:
<a href="#wiring">- Wiring Diagram</a><br>
<a href="#arduino">- Arduino Codes</a><br>

The haptic-joystick library can be downloaded using git:

    git clone https://github.com/makerportal/haptic-joystick

<a id="wiring"></a>
# - Wiring Diagram -
Here, we are wiring the analog joystick module and buzzer to GPIO pins on the ESP32 D1 Mini board:

![ATGM336H wiring to ATSAMD21](/images/atgm336h_datalogger_wiring.jpg)

![ATGM336H wiring to ATSAMD21 - table](/images/atgm336h_datalogger_wiring_table.jpg)

<a id="arduino"></a>
# - Arduino Code -
The Arduino code used to log GPS data is found at:

- [gps_datalogger.ino](/arduino/gps_datalogger.ino)
