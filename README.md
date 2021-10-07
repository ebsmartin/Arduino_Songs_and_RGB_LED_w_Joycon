# Project1_Arduino_Songs_w_Joycon

Utilizing the X Y Axis potentiometers within an analog joystick, I have created a simple device that allows the user to manually change the color of an RGB LED depending on the position of the joystick. When the joystick is depressed, depending on the position when depressed, a unique song will play as well.



Creating Things That Think
Project 1
Eric Martin
September 14, 2021
IDEA 310L

**Description of Design Process**

Design requirements :
- Using at least two inputs
- Using at least two outputs

Design Process :
- Want to implement joystick as an analog input
- Want to implement LED’s
- Want to implement sound
- Want the design to look nice and compact


**Songs :**
1. Final Fantasy Victory Fanfare
2. Game of Thrones Theme
3. Hedwig’s Theme Harry Potter
4. Imperial March Star Wars
5. Mario Theme Song
6. Jigglypuff’s Song Pokemon
7. Keyboard Cat Meme Song Youtube
8. Greensleeves Skyrim

**Issues :**
- When activating some songs, the LED turns off.
  - Usure about why this is occurring as each melody has the same outline of code.
 - Program global variables use 79% of the dynamic memory on the heap which leaves less memory and could lead to stability issues.
  - This is caused by the large amount of melody variables declared not using progmem()
- Light transitions when using the joystick are sometimes jumpy rather than smooth.
  - This may be due to the limitations of the joystick input or the translation from analog to digital input.
- Box is flimsily and makes using the joystick harder than it needs to be
