# SimHub Profiles for FRG

I'm providing some sample meter configurations for the FRG in SimHub

They're provided in separate folders because SimHub manages both components separately.

Video with some samples:
https://youtu.be/f9Xryb7ePtg

## RGB-LEDs
In this folder you can find the "RGB Leds" tab profiles for the meter ring of LEDs. You can import these configurations from SimHub's UI directly and even pick specific games you want the configuration applied. 

Keep in mind that these profiles don't include your current configuration for LEDs, which means if you have a wheel that uses simhub for its effects, this will not include those effects. In order to keep all current effects, make sure your meter is NOT the first device in the list of arduinos, and add the same effects that these profiles use, but offset by however many LEDs your higher priority devices have. Example: you have a wheel with 16 LEDs; connect your gauge, let it be recognized by simhub, make sure it's the second device (LEDs 17-40), create a new LED effect that starts with LED #17 and LED count of 24.

To use
 - Go to the "Arduino" section, 
 - Go to RGB Leds tab
 - Click "Profiles manager"
 - Select the icon to "Import Profile"
 - Pick the profile file you want to import
 - You can edit it to apply it specifically to a game, or be active for all games.
 - Customize colors, brightness or values
 - You can click "Open test data editor" to set some test values and checkout how it looks

## OLED
In this folder you can find configurations for the OLED screen. 
To use
 - Go to SimHub's installation folder (typically C:\Program Files (x86)\SimHub)
 - find the folder called "OLEDTemplate". This folder contains the drawing configuration used for the LCD and OLED screens.
 - Make a copy of it somewhere
 - Pick a configuration from the OLED\Ingame folder in this repository
 - Copy the folder to your "OLEDTemplate\Ingame" folder in the SimHub installation
 - Rename the folder with the appropriate number, try to keep them in sequence
 - The folder that you name "0_{something}" will be picked as the default screen when games data is received by SimHub
 - You can move between configs by setting up simhub to do so in "control and events" section. Your screens will appear under the "Oled_XXXXXX" targets

Read more about OLED drawing configs here:
https://github.com/SHWotever/SimHub/issues/571

