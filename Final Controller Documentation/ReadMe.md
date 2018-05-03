# Controller Documentation
## In the last documentation...

The last thing I said I wanted in the midterm documentation was to add another IR sensor to my assembly, and perhaps another sensor. I was having difficulty figuring out why the keystrokes were not behaving as a keyboard would, and instead as hundreds of individual key pushes. This was incompatible with games.

## Build Changes and Solutions

I changed the Leonardo to a Micro to keep the device compact, and because it was cool looking.

<html>
<img src="https://github.com/BeccaHa/Digits2018/blob/master/Final%20Controller%20Documentation/Gesture.jpg">
</html>

I finally found this forum post, which addresses the keyboard recognition problem, pointing out that there is a keyboard.press(), which behaves like a held down key. This is opposed to keyboard.write(), that I was using. 
http://forum.arduino.cc/index.php?topic=152623.0

## New Sensors

Swapped out the IR sensor for the Adafruit gesture, proximity and color sensor. Swiping is now movement. 


<html>
<img src="https://github.com/BeccaHa/Digits2018/blob/master/Final%20Controller%20Documentation/GestSen.jpg">
</html>

It took a little bit to get the behavior of this right. I tried making a close proximity act as a hard stop to all gesture input, but couldn't get that to operate at the same time as a gesture functionality. 
Ended up using a button for that task.

## Add a Mouse

I added the joystick I was originally planning on using, and made it behave like a mouse (computer). This allows me to use the controller on games requiring the mouse to look around. Pressing the joystick is treated as a mouse click. 
I also added a few more buttons

## Hardening

I sautered it all together, and wrapped it in plastic for casing, keeping the electronics visible. This is partially for necessity, because I can't figure out how the best way to box up the gesture sensor. It doesn't work well through clear plastic.


<html>
<img src="https://github.com/BeccaHa/Digits2018/blob/master/Final%20Controller%20Documentation/Sauter.jpg">
</html>


<html>
<img src="https://github.com/BeccaHa/Digits2018/blob/master/Final%20Controller%20Documentation/Controller.jpg">
</html>

Then I changed my mind, and wrapped it in some scrap leather I had around. This has a good feel to it, and the controller doesn't feel too bulky in the hand. 


<html>
<img src="https://github.com/BeccaHa/Digits2018/blob/master/Final%20Controller%20Documentation/LeatherCase.jpg">
</html>


## Functionality

https://drive.google.com/file/d/1NrR11G777Wo0QvvvL_hKZc__d_2pGJ3k/view?usp=sharing

## Future

I plan on creating a better housing for the system, and perhaps I'll reapproach the design some day to include more inputs. There are still a few kinks I need to work out... the "mouse" lags after a few minutes of being plugged in, I'd like to get that proximity sensor multitasking working, and I could add some debouncing to the various clicks and presses to make work smoother, i.e. knowing when to click and with to hold down the mouse button on something.

Good Project. Good fun.
