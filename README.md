# Open Arduino RC Car
Hello, Welcome to the project page for Open Arduino RC Car project I have been working on for the past few months. I wanted to make a remote-contolled car using the Arduino microcontoller platorm, but I could not find any suitable tutorials that included beginner-frienly coding concepts or utilizing budget-friendly parts that are easy to scource. Considering these obstacles, I decided to create the entire RC car from scratch, and here it is. Below is an extensive documentation of the circutry and Arduino sketches. 

## Electronic Components

### RC Car
* Arduino MEGA R3 Board - The larger number of digital pins allows for more IO devices
* 9-Volt Battery - To power the Arduino Mega
* HC-SR04 Ultrasonic Distance Sensor - To avoid crashes in autonomus operation 
* Piezzo Buzzer - Makes a sound on startup 
* Tilt Ball Switch - To detect if the car has flipped over
* NRF24L01 Wireless Transceiver & Antenna - For communication with the remote 
* L298N Motor Driver Controller Board - To controll the DC motors
* 4x Yellow DC Hobby Motors - You can guess what these are for
* 2x Rechargable 650mAh 9-Volt Batteries - To power the driver board and motors
* Rocker Switch - For turning the car on and off

#### Notes: 
With the main focus of the project being to remain budget-friendly, I opted for rechargable 9-Volt batteries becasue using single use batteries can be quite expensive over time. They are wired in paralell at 9-Volts so that the 5-Volt regulator on the motor driver board wont overload. I chose the NRF24L01 in specific because it can act as a transmitter as well as a receiver, which opens the possibility of sending information back to the remote (for autonomus mode). The antenna extends the range of communication to farther than 500 feet, which will be more than enough for the project. 

### Remote Control
* Arduino Uno - Small enough to fit in the remote body, with enough IO pins to connect the controls
* 2x Dual-Axis Joystick Modules - For contolling the motors
* NRF24L01 Wireless Transceiver & Antenna - For communication with the car
* 2x Heavy Duty Toggle Switch & Cover - Added control and looks awesome 
* 9-Volt Battery - To power Arduino Uno
* Rocker Switch - For turning the remote on and off

#### Notes: 
The biggest design challenge of the remote was getting all the components to fit into the small formfactor. Although smaller than the Arduino Mega, the Uno takes up a considerable amount of space, and the placement of the other components was designed around it. Since the joysticks can move left and rick as well as up and down, there are alot of possible steering dynamics (One for forward/backward and the other for left/right, or each for one side of the car - tank steering). 

## Mechanical Components 

For this project, I decided to 3D print all of the mechanical compontents becasue I can easily replace broken parts as well as modify them when needed. 3D printed parts are also very cost-effective, with all of the parts being printed in PLA filament on my Ender 3 V2. 

### Remote Control










