  
  Library for use RFID tags with RDM630 module in UART usage.
  Created by Danilo Queiroz Barbosa, August 26, 2016.
  Member of electronicdrops.com
  Released into the public domain.


 The module is RDM630 and has two data formats. UART and Weigand. This library only works with UART data format.
 The frequency is 125Khz and compatible with EM4100 TK4100 EM/TK4102, EM4200



DATA FORMAT:

14bytes

STX(0x02) DATA(10ASCii) LRC(2ASCii) ETX(0x03)


PINOUT:

_____________________
|           P1 *****|
|                  1|
| 1                 |
|** P2        P3 ***|
|__________________1|


P1:
1 - TX
2 - RX
3 -
4 - GND
5 - +5V (DC)

P2:
1 - ANT1
2 - ANT2

P3:
1 - LED
2 - +5V (DC)
3 - GND


 -  To use, connect VCC, GND on the respective pins.
 -  The connect P1:1 of RDM630 module on Arduino Pin 6  tx-rx
 -  If you wanna use Interupt, conect P3:1 of RDM630 module (LED pin) on Arduino Pin 2.




