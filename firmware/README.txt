Code is in c++ intended for esp32 devkit v1
Please recheck the library version, anyways here's a wiring instruction
INMP441 - ESP32
VDD - 3.3V
GND - GND
SCK - GPIO32
WS - GPIO25
SD - GPIO34
L/R - GND
WS2812B LED STRIP
DIN - 300Ω → GPIO13
GND - GND
MT3608 boost converter (use a multimeter to check the boost and adjust first prior to adding electricity)
+Vout - led strip 5v pin
-Vout - GND
Lipo battery (preferably 20 000mah)
Splice the red wire before connecting it to the boost converter and connect it to ESP-32 VIN pin
Red wire - MT3608 +Vin pin
Black wire - GND
Splice all GND together and add solder and a electrical tape!!!
Refers to the schematic down below for more indepth guide.
