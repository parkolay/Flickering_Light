# Flickering_Light
This is for the DigiSpark w/ 3 WS2812 LEDs, more of less WS2812's could be added or removed (there is more of a limit using the tiny85 because of memory) Code was taken from the the Adafruit NeoPixel example, there were some issues using the DigiSpark but those were fixed and serial connection was removed (DigiSpark does not use the serial terminal like "normal" Arduino projects).

Extra Help connecting the DigiSpark if you haven't done it before;
http://digistump.com/wiki/digispark/tutorials/connecting
(read the fine print about downloading the drivers if you are using a Windows OS, I had to grab them and install manually, the auto get didn't work for me)
Also read the programming bit about having to start the download THEN connect the board, this isn't intuitive but necessary.

Remember to grab the library files :)

Also remember to follow the best practices as laid out by Lady Ada
(https://learn.adafruit.com/adafruit-neopixel-uberguide/best-practices)
Before connecting NeoPixels to any large power source (DC “wall wart” or even a large battery), add a capacitor (500–1000 µF at 6.3V or higher) across the + and – terminals as shown above. The capacitor buffers sudden changes in the current drawn by the strip.
Place a 300 to 500 Ohm resistor between the Arduino data output pin and the input to the first NeoPixel. The resistor should be at the end of the wire closest to the NeoPixel(s), not the microcontroller. Some products already incorporate this resistor…if you’re not sure, add one…there’s no harm in doubling up! Also, newer NeoPixels are less picky about this. Nothing’s needed at the “out” end of a strip…you can leave the data out “floating.”

Not following this could have been the reason I blew out one of the WS2812s in my (Santa) project
