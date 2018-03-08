# Midterm Documentation

## Game Controller
### Concept: create a method of game control

I originally sought to make a controller using an Arduino Uno by tricking the computer into thinking that it was a game controller. This involved use of method called UnoJoy that I found. It led me to old software and outdated programs, and ultimately didn't pan out. This entire process caused me to use a lot of time NOT on the actual arduino, setting me back a little ways.

I finally found that there are a handful of arduino boards that already can work as USB devices, such as the Leonardo and the Micro. There was another week of time spent sautering a borrowed Leonardo board, and making sure that I could get it to work with the computer

After initial testing, done with three buttons meant to type a, w, and s ( the right, forward, and left controls on a keyboard based game), I made the mistake of not turning off the output in the code, causing an endless loop of letters to spill out whenever I had the arduino plugged in. AFter finally getting the timing right to reset the board, I instead attached the buttons to lights to make sure they turned off afterwards. Then I introduced the actual keyboard functionality with success.

#### Three Button Set-up

<html>
<img src="https://github.com/BeccaHa/Digits2018/blob/master/MidtermDocumentation/threeButtonDoc.jpg">
</html>

From there I wanted to add some complexity to the controls themselves, so I replaced one of the buttons with a IR distance sensor. I programed it so that when my hand was close to it, it outputted a w, and when my hand was far, it outputted an s. I left two buttons to act as A and D. 

#### IR Distance Set-up

I connected each output also to an LED so I would know when it was sensing what as it came time to test the system with actual games. I found, however, that when I held down a button, or left my hand in one position over the distance sensor, even though a continuous stream of letters would be produced as desired, movement didn't happen in games. I was able to make a menu function, but the arduino interpretted a stream of letters as a bunch of isolated key presses. I was told that I should learn the debounce() command to fix this problem.

