# ECE 387-Form Correcting Knee Brace
This project is an embedded system that assists users by monitoring knee instability during physical activity to ensure safe and proper rehabilitation. This project was done using an Arduino microcontroller but can be implemented on an RPI or other simliar microcontrollers with a little tweaking. 

# Description
The Correcting Knee Brace is built from an athletic knee brace, the LSM9DS1 accelerometer-gyroscope, 5 LED's, and five 1Kohm resistors. The LSM9DS1 was mounted to be alligned with the users knee to track the motion of the knee. The LED's were placed at five points around the front front of the knee. As the LSM9DS1 dectects that it is "falling" or tilting too much in one direction, it will prompt the microcontroller to light the LED corresponding to the direction it is tilting in.

# Purpose
After tearing my own ACL, one of the hardest parts about doing physical therapy on my own was making sure that I was doing the excerises properly. After surgery, my knee was especially weak, buckling often while I was exercising. Trying to focus both on the exercise and getting my weak, uncorrdinated muscles to do what I wanted felt like too much at times and I often wished that there was a way I could mend this. The brace was the solution to this problem. When your muscles and ligaments are healing after a serious injury, most of the time you are not moving exactly how you think you are and the knee brace is meant to provide the user with a corrective visual.

# How it's Built
The LSM9DS1 accelerometer uses I2C, so using the SCL and SDA pins are all you need to get your data. Wiring them to the Arduino's serial clock and data pins will enable your data stream and wiring it to 3.3V and ground will ensure a safe operating voltage. Each LED is wired to a digital output pin. The five LEDs and the accelerometer were stuck into a strip of cardboard that wraps around the front of the users knee. All the connection points not on the arduino itself were soldered. Here is a link to the demo of the final project.
https://www.youtube.com/watch?v=57nDac-gl3w&feature=youtu.be
The Jpeg files in the repository are the design plans I made before implementing my project. The plans are more complicated than the actual implementation, but the main design holds and is fully functional.




