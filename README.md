# haptic-joystick
Haptic joystick buzzer with Arduino - creating different buzz patterns for different joystick movements with ESP32 arduino board

Get an Analog Joystick module here: [Analog Joystick Module](https://makersportal.com/shop/mini-gps-module-atgm336h-antenna) <br>
See full tutorial here: [Haptic Feedback Joystick with Arduino](https://makersportal.com/blog/haptic-feedback-joystick-with-arduino) <br>

# 
### JUMP TO:
<a href="#wiring">- Wiring Diagram</a><br>
<a href="#arduino">- Arduino Code</a><br>

The haptic-joystick library can be downloaded using git:

    git clone https://github.com/makerportal/haptic-joystick

<a id="wiring"></a>
# - Wiring Diagram -
Here, we are wiring the analog joystick module and vibration motor to GPIO pins on the ESP32 D1 Mini board:

![Haptic Joystick + ESP32 wiring](/images/wiring_diagram.png)

The wiring table is also given below for reference:

<table class="tg" style="undefined;table-layout: fixed; width: 502px">
<colgroup>
<col style="width: 201px">
<col style="width: 150px">
<col style="width: 151px">
</colgroup>
<thead>
  <tr>
    <th class="tg-qblo">ESP32</th>
    <th class="tg-qblo">Joystick</th>
    <th class="tg-qblo">Vibration Motor</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-nqrr">3V3</td>
    <td class="tg-nqrr">+5V</td>
    <td class="tg-nqrr"></td>
  </tr>
  <tr>
    <td class="tg-g1p2">5V</td>
    <td class="tg-g1p2"></td>
    <td class="tg-g1p2">VCC</td>
  </tr>
  <tr>
    <td class="tg-nqrr">GND</td>
    <td class="tg-nqrr">GND</td>
    <td class="tg-nqrr">GND</td>
  </tr>
  <tr>
    <td class="tg-g1p2">D34</td>
    <td class="tg-g1p2">VRX</td>
    <td class="tg-g1p2"></td>
  </tr>
  <tr>
    <td class="tg-nqrr">D35</td>
    <td class="tg-nqrr">VRY</td>
    <td class="tg-nqrr"></td>
  </tr>
  <tr>
    <td class="tg-g1p2">D14</td>
    <td class="tg-g1p2">SW</td>
    <td class="tg-g1p2"></td>
  </tr>
  <tr>
    <td class="tg-nqrr">D2</td>
    <td class="tg-sr7s"></td>
    <td class="tg-nqrr">IN</td>
  </tr>
</tbody>
</table>

<a id="arduino"></a>
# - Arduino Code -
The Arduino code used to control the vibration motor based on joystick movements is given at:

- [haptic_joystick.ino](haptic_joystick.ino)
