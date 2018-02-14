# CompassRobot
 Robot, walking on the freedom of direction (north, south, west, east). .NET Micro Framework (С#) &amp; I2C Protocol is used.
 
 
 
 
Programm.cs: 
The robot goes in the right direction the right time.
Klichko.Go(x,y)  //x - angle of motion (0-360 degree), y - time of motion;


Robot.cs:
The Go () method calculates the speed of the left and right axes, if the left goes to the full (1), and the right one stands (0), then the robot simply turns to the right. The Compass class is used to communicate with the compass via the I2C protocol. To calibrate the compass so that 0 is straight, and 90 is right, the CurrentDegree () method is written, the Calibration enumeration is added to the beginning of the code for convenience;

