# Problem description
According to the Chinadaily.com.cn, each year approximately 260,000 people experience and die from the car accidents, and around 6 in 10 of the total estimated deaths are pedestrians in China. Around the world, there is 1.25 million people die from road traffic injuries each year with 20 to 50 million people sustain nonfatal injuries. 
Moreover, Road traffic injuries are a top 10 reason of death globally, especially individual age between 15 and 29. Even though automations have a precaution sensor when it nears something, it just the sound.

Therefore, the experiment regarding the car model, the function is to follow the wall on the right side. When it is nearly bumps the wall, it will change the direction. By inserting ultrasonic sensor which measuring the distance from the object, this can be very helpful for avoiding the obstacle. Additionally, it can be improved to be more effectivity, so it can avoid object not only, in front, but also surrounding. This will increase the safety in society.

# Design concept
The concept for the car model is to prevent the car from barricade. This car model consists of an ultrasonic sensor, a servo, 2 DC motors, an Arduino, a breadboard, a 6V battery, and a H-bridge. The sensor that is added can detect only the object in the front with the distance that is set. In addition, to avoid the object on the right or left, servo can spin the sensor. Therefore, the input is ultrasonic sensor that can rotate, and the output is the car’s motion when it meets obstruction. 

 <img width="338" alt="image" src="https://github.com/user-attachments/assets/22c6e990-88c2-48a0-83c0-d2fbb80096c2">

# Analysis of Components 
## Characterization of each sensor
The main component of the design is ultrasonic distance sensor (HC-SR04). Its operation is to calculate the distance in front of it by emitting the sound waves at a frequency that human is unable to hear and wait for the wave to reflect. Then, the ultrasonic distance will know the if there is an item nearby. Hence, it can prevent the car not to collide with other barriers. Other components using in this car model is servo. The servo is mechanism that control the rotational and position. This is the reason why servo is used to make the sensor have an ability to turn and act like a neck. 
 
<img width="146" alt="image" src="https://github.com/user-attachments/assets/dbefc545-a349-4ad2-8cdb-18e6834e2036"> 
      Figure 1: The output of the oscilloscope's DC motor.
      
<img width="99" alt="image" src="https://github.com/user-attachments/assets/9174b29e-121a-405a-9ed3-a43751ca3c4e">
      Figure 2: The output of the oscilloscope’s servo.         

<img width="99" alt="image" src="https://github.com/user-attachments/assets/3d86d98f-b5cc-4d46-a631-76b5fa94802d">
      Figure 3: The output of multimeter 

## Design considerations
Once the circuit is powered and connected to the Arduino, the operation will begin, and the car will start moving. When the car approaches an obstacle, there is a distance threshold set by the user in the Arduino code. An ultrasonic sensor sends a signal to the Arduino when the distance of an obstacle falls below this threshold. When the Arduino receives a signal from the ultrasonic sensor, it sends a signal to the motor as well as the driver to stop the motor from spinning.
Consequently, signal will be sent to the driver again and turn the car left or right is dependent on the servo corporate with ultrasonic sensor. Then the car will make a turn and start moving forward again and continues forward until it finds another obstacle. Repeat the above operations until the power is turned off.

# Design Description 
## Block diagram 
![image](https://github.com/user-attachments/assets/afb8c01c-d691-48fb-bbda-5dbb53a5a4e3)

## Circuit schematics  
![image](https://github.com/user-attachments/assets/5c16323f-9e62-4fa0-b52e-c53eb7f15a45)
<img width="455" alt="image" src="https://github.com/user-attachments/assets/2cfad20a-a054-450f-8a37-451c8ea98d0c">

## Physical/mechanical construction
![image](https://github.com/user-attachments/assets/12508b43-211d-4fba-a03b-416f5df22649)

# Conclusion 
Lessons learned
Although doing electronic lab online seem easy, I have approached several inevitable problems. The main issue of construct this model through an online platform is measure components via online device. This is difficult since I need to build a circuit and make it be able to run before making a measurement. The program that I use it cannot import library, thus I need to rewrite the whole code, learn more regarding coding.  Furthermore, some electronic components are not exit in this program. The solution I can do is find an alternative component and replace with a similar operation. 

Self-assessment
Now that I have finished my circuit , I have learned numerous lessons from this project that increase my confident in this study field. My circuit’s design seems to be smaller than the problem scale. However, it can be a very good initial phase for a further development.
