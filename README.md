# Wavecoustic

An ESP-32 with INMP441 mic to analyse piano sound using FFT (Fast Fourier transform) to light up WS2812B led on the corresponding across the piano key.

## Description

This is a controller for a LED strip that lights up a piano key when pressed. I know a version of this had been done before; however, as far as I know, there had only been a version where the input for the LED was from MIDI, which is impossible to do with an older piano or an acoustic piano. I wanted to make this project so much because looking back I would have practiced the piano so much more if it wasn't so boring. So, my goal is to use an actual microphone input and FFT to translate the sound wave signal into individual key notes. So that it becomes fun and usable. 

## Getting Started

### Usage

* Place the 1.4m led strip over the piano in possition.
* Charge your external LIPO-battery using Tp4056 usb-c charging module.
* Plug the external lipo battery in and rest it on the holder (please be aware of the polarlity).
* Set the setting mode and brightness via esp32-accesspoint captive portal.

### Assembling

* The text on the silk screen corresponse to the schematic so soldering should be easy.
* Please flash the attiny before you solder it.
* Solder all the smd first, then add the resistor and capacitor based on the silk screen.
* Hold down those with tape then solder it. Finally solder the attiny, shift-register and power components.
* Connect the lipo battery and put it under the pcb.
* Slide in the wrist strap through the pcb hook.
  
### Firmware

* 
* 
* 
* Sidenote I'm not really sure about the code but I tried my best to polish it because my friend quit half way.
```

```
### ISP programing
* Use any Arduino (but for this example I'm using UNO)
* Requires: jumperwire, breadboard, 10uF capacitor, usb type-B for com to arduino.
* While uploading isp to arduino unplug the capacitor then put it back in after you complete the upload.
* For more information read here: https://www.hackster.io/arjun/programming-attiny85-with-arduino-uno-afb829
* However, the tutorial have a flaw where he connect the capacitor anode to GND DONOT follow it.
```
Attiny85 to Arduino Uno 
pin 1 -> Digital Pin 10
pin 5 -> Digital Pin 11
pin 6 -> Digital Pin 12
pin 7 -> Digital Pin 13
pin 4 -> GND
pin 8 -> 5V
* Add a 10uF capacitor between RESET and GND in arduino to avoid arduino resetting.
```

## Materials

This is the BOM of the pcb, most of them are a through hole component.
For the Lipo and wriststrap you can use whatever components you want.
```
| No. | Component | Qty |
| 1 | 100nF Capacitor | 5 |
| 2 | 12pF Capacitor | 2 |
| 3 | 4.7uF Capacitor | 2 |
| 4 | JST B2B-PH-K-S Connector | 1 |
| 5 | SMD LED (13 blue, 1 red, 1 green) | 15 |
| 6 | 330Ω Resistor | 15 |
| 7 | 10kΩ Resistor | 1 |
| 8 | 20kΩ Resistor | 1 |
| 9 | 5.1kΩ Resistor | 2 |
| 10 | SMD Tactile Switch | 1 |
| 11 | 74HC595N Shift Register | 2 |
| 12 | ATtiny85-20PU | 1 |
| 13 | MCP73831T-2DCI/OT Charger | 1 |
| 14 | TYPE-C 6P USB Connector | 1 |
| 15 | 32.768kHz Crystal | 1 |
| 16 | LiPo Battery ~100mAh *(DNP)* | 1 |
| 17 | Wrist Strap 20cm *(DNP)* | 1 |
```

## Assembled Pictures

## Rendered Pictures

## Captive Portal interface
<img width="373" height="445" alt="Screenshot 2026-06-18 032915" src="https://github.com/user-attachments/assets/ff6574ff-b611-4831-ab5b-705859b5a18c" />


## Schematic 
<img width="1769" height="1251" alt="SCH_Schematic1_2026-06-14 (1)_page-0001" src="https://github.com/user-attachments/assets/8684b099-6665-4e5c-9a5a-702e105f07e2" />


# Zine Poster
<img width="1410" height="2000" alt="waaavecoustic (1)" src="https://github.com/user-attachments/assets/4f861a55-da71-4618-9970-9b8e22a6dd7f" />



