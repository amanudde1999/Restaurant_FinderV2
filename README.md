# Restaurant_FinderV2
Description: The second part of this assignment involves the use of the joystick to move the cursor around the map displayed on the TFT Display, you can also view which restaurants are near you in Mode 1 and find out exactly where they are on the map. Moreover, there are now two buttons, one on the top right and one on the bottom right of the screen. These will restrict the restaurant choices depending on the rating the top right button displays and the sorting algorithm will change depending on the bottom right button.

Included files in this are:
-----------------------------
- a1part2.cpp
- README
- Makefile
- lcd_image.cpp
- lcd_image.h
- restaurant.cpp
- restaurant.h
- yegmap.cpp
- yegmap.h


Required Components:
--------------------
- 1 x LCD Screen
- 1 x Arduino MEGA 2560 Board
- 1 x Arduino USB cable
- 5 x Jumper Wires
- 1 x Joystick 

Wiring Instructions:
-------------------------

| Joystick Pins | Arduino Pins |
| ------------ | ------------ |
| VRx | A8 |
| VRy | A9 |
| SW  | Digital Pin 53|
| GND | GND |
| +5V | 5V |

- Arduino <--> LCD Screen


Running Instructions:
-----------------------
- Use the "arduino-port-select" to ensure that the connected Arduino is port 1 for both.
- Open the directory containing joy_cursor.cpp file in the terminal window. Use the "make upload a1part1.cpp" to upload the code to the Arduino. Once the map fully loads on the LCD screen, you are now able to use the joystick to control and move the red cursor around the map.
- This is mode 0, if you go over any parts of the map, a new patch will be loaded and you will be able to move around there too.
- If you tap on the screen, you will be able to see which restaraunts are currently on the same patch as the one you are on and they will be 
displayed as black dots.
- To enter Mode1, press the joystick and a screen will load with 21 of the restaraunts near you, you can use the joystick to scroll down and up the list of restaraunts, once you select the restaraunt click the joystick and the map will reload with the cursor near the selected restauraunt.
 - Clicking on the rating button (top left) will increment it, this will restrict which restauraunts will now appear, say for example the rating button was incremented to 4, it will only display 4 and 5 star rating restaraunts in the area. The ratings go up to 5 stars.
 - Clicking on the bottom right button allows you to choose which sorting algorithm you which to use: quick sort, insertion sort or both. It will also display the running time for both in the serial monitor, which you can open via the comman terminal using "serial-mon" command.


