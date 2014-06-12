========
TDH board bringup debugging log

--------
MFG 
1.MX6Q seems must support 528MHz DDR(DDR3 or LPDDR2) timing,otherwise it can't jump to OS successfully.
After replace it to MX6DL,default 400MHz LPDDR2 can going up.

--------
Keyboard(button)
OKAY

--------
USB 
1.USB HUB does not work because upstream port shorted with one of downstream port.

--------
LCD
1.128 bytes command and data can not send to LCD successfully,after splitting it to 4x32bytes,it's okay;
2.LCD display not okay for unknown reasons;


--------
TouchPanel

--------
Power(Charging&Battery)

--------
WiFi
1.No wifi module founded in first rework board;

--------
GPS

--------
Audio Codec


--------
SD card
OKAY

---------
Camera

---------
Flashlight

---------
4G



