**Read me "Punch-A-Scroll" Led Sequence and Manual Control Code **

**Date of Creation: ** 15.10.2025
**Most recent edit:** 21.10.2025
**Creator: **Silja Marti, 2228912

**Description:**
This Arduino project controls multiple LED strips to run a set sequence of colored flashes. The sequence includes:
A start animation
red LED flashes
Interrupting white flashes triggered by button presses
A rainbow ending sequence


**Hardware:**
- Arduino Uno 
- WorldSemi WS2812B Digital 5050 RGB LED Strips (2 strips with 8 leds each and 1 strip with 12 leds) + one 331 Ohm resistor for each strip
- 3 Small Push Buttons 
- Breakout module: USB-C Breakout Sparkfun BOB-15100 
- Depending on your set up, about 21 meters of alpha wires (red (5V), black (GND), white (Data))

**Libraries used: **
Adafruit_NeoPixel.h 

**Usage:**

1. Connect the LED strips and buttons to the Arduino pins defined in the code
2. Power your LED strips via the breakout module with a powerbank or with a PC
2. Upload the sketch to the Arduino  
3. Press the **start button** to begin initiating sequence 
4. Press the **start button** again to initate LED sequence
4. Press **punch buttons** during the sequence to trigger white flashes  
5. Feel accomplished during the rainbow celebratory phase 

**References: **
1. Led set up: https://adafruit.github.io/Adafruit_NeoPixel/html/class_adafruit___neo_pixel.html#details 
2. Variable used for interrupting logic (used with millis): Arduino documentation: https://docs.arduino.cc/language-reference/en/variables/data-types/unsignedLong/ 
3. Interrupting Led logic: OpenAI. GPT-5-mini. Prompt: "Example of a logic that interrupts a set led sequence with a flash (other colour) by pressing a button (arduino)"
4. Interrupting led logic: Arduino library. https://docs.arduino.cc/language-reference/en/functions/time/millis/ 
5. Rainbow sequence: Adafruit common utility functions: https://learn.adafruit.com/multi-tasking-the-arduino-part-3/utility-functions 
6. Rainbow sequence: Adafruit forum: https://forums.adafruit.com/viewtopic.php?t=123034 

