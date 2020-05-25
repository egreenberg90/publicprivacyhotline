# publicprivacyhotline
These instructions are for creating an old analog phone that rings in response to motion. When someone picks up the phone, it stops ringing and begins playing a custom music track.

Materials:
Arduino
Sparkfun MP3 shield
Breadboard
Wires, resistors, LED
An old phone you don't mind destroying - I like the Cortelco phones and have also used a public payphone.
Headphones you don't mind destroying - I like to use cheap over the ear headphones
Button - better to use the one in the phone
MicroSD card for storing music tracks
PIR motion sensors
Soldering tools
Processing software
USB Charger

This is a helpful resource for working with the MP3 shield:
MP3 player Shield Hookup Guide
https://learn.sparkfun.com/tutorials/mp3-player-shield-hookup-guide-v15?_ga=2.235145409.138964658.1554038927-1783721443.1554038927

Basic instructions:
Solder pins to the MP3 shield
Record some tracks, format per the Hookup Guide, and put the MicroSD in the shield
Attach to Arduino
Set up the breadboard as I have in the jpeg. It should be connected to a power source, headphones, a PIR sensor, and a button. At this stage, just use a regular arduino button. 
Note that you can adjust the sensitivity of the sensor.

***Before setting up the breadboard, test each component in isolation. You can find very simple code for these with a quick Google search. 
Get the arduino to play music tracks through the headphones: https://learn.sparkfun.com/tutorials/mp3-player-shield-hookup-guide-v15/all 
Test that your button works: https://www.arduino.cc/en/tutorial/button
Test that your PIR sensor works: https://learn.adafruit.com/pir-passive-infrared-proximity-motion-sensor/using-a-pir-w-arduino *****

In Processing, paste in the code I have included in the files. Do proper testing to ensure it works. Note that you will want to play around with the volumes. The ringing should be much louder than the tracks you listen to with the phone pressed against your ear.
Once the electronics are working, it's time to get it working in the phone itself. Unscrew the bottom of the phone. You'll want to get rid of the phone guts. Take out everything except the wires connecting to the button where the headset rests, and leave the headset alone for now.
It's best if you can figure out the wiring of the phone button (where the headset rests) and sub that in for the other button. If not, you will have to make the phone button physically press the button you are hooking up to the breadboard. 
It's also nice if you can hack into the phone speakers, solder them to a jack, and plug in, but this is a little tricky. Using already existing headphones is quick and will get the job done. Just open up the headset and take everything out. Now take apart your headphones. You will want to remove the part that rests on your head and all the padding that surrounds the actual speakers. When you're through, you should be left with the speakers and the wires connecting to the jack. Shove this into the headset and position the speakers where you would normally hear them in the top circular part of the phone. Thread the cord in the coil of the actual phone cord and plug the headphone jack into the MP3 shield.
Shove all the electornics in the phone, close her up, and plug in!
