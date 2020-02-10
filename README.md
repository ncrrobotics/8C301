Our first project is the 8C3 controller option database

Start with some definitions
Degrees of freedom robotics definition
A common term in robotics is "degrees of freedom," which describes the technical number of axes in which a robot can operate. The more degrees there are, generally the more flexibility and options are available to the user.
 
For this first project I use 3 degree of freedom robotic arms or 3DOF. Different degrees of freedom can be used with less controller options. So you could have a more diverse range 12dof with 3 controller options would give 3C12.

To view the possibility matrix of controller and degrees of freedom we can use the nCr and nPr equations to calculate combinations and permutations.
 
Definition of Combinations and Permutations

Permutation:
In a set all of the order specific combinations are each permutation so ab does not equal ba they are separate permutations
 
Combination:
The combinations within a set that is not order specific so ab=ba
 
Let a, b, c be three letters. From this clearly, six different arrangements can be made by taking two letters at a time, example: - ab, ba, bc, cb, ca, ac; each of these arrangements is a permutation. Then, three different selections can be formed by taking two letters at a time example: - ab, bc and ca; each of these selections is a combination. Please note that, an order must be considered in forming permutations (i.e., ab and ba denote different permutations); but an order is immaterial in forming combinations (i.e., ab, and ba denote the same combination).
 
Controller options
1) C Arduino program
2) Joystick
3) Potentiometer
4) Button
5) Rotary encoder
6) Ir remote
7) Serial monitor
8) Tablet blue tooth

So in the formation of the combinations of controller and degrees of freedom we can calculate that 8C3 = 56 and 8P3 = 336. The permutations has a higher amount of possibilities as the degree of freedom order is specified so a combination could be.
  
The combinations are

1,2,3          Program, Joystick, Potentiometer
1,2,4          Program ,Joystick, Button
1,2,5  	      Program, Joystick ,Rotary Encoder
1,2,6          Program, Joystick ,IR Remote
1,2,7 	      Program, Joystick, Serial Monitor
1,2,8	      Program, Joystick, Bluetooth
1,3,4	      Program, Potentiometer, Button
1,3,5	      Program, Potentiometer, Rotary Encoder
1,3,6	      Program, Potentiometer, IR Remote
1,3,7         Program, Potentiometer, Serial Monitor
1,3,8         Program, Potentiometer, Bluetooth
1,4,5	      Program ,Button, Rotary Encoder
1,4,6         Program ,Button ,IR remote
1,4,7         Program, Button ,Serial monitor
1,4,8	      Program ,Button ,Bluetooth
1,5,6         Program ,Rotary Encoder ,IR remote
1,5,7         Program, Rotary Encoder ,Serial Monitor
1,5,8	      Program, Rotary Encoder ,Bluetooth
1,6,7	      Program, IR remote ,Serial Monitor
1,6,8	      Program ,IR remote ,Bluetooth
1,7,8	      Program ,Serial Monitor, Bluetooth
2,3,4	      Joystick, Potentiometer, Button
2,3,5	      Joystick, Potentiometer, Rotary Encoder
2,3,6	      Joystick, Potentiometer,  IR Remote
2,3,7	      Joystick, Potentiometer, Serial Monitor
2,3,8	      Joystick, Potentiometer, Bluetooth
2,4,5	      Joystick, Button, Rotary Encoder
2,4,6	      Joystick, Button, IR Remote
2,4,7	      Joystick, Button, Serial Monitor
2,4,8	      Joystick, Button, Bluetooth
2,5,6	      Joystick,  Rotary Encoder ,IR Remote
2,5,7	      Joystick ,Rotary Encoder ,Serial Monitor
2,5,8	      Joystick, Rotary Encoder ,Bluetooth
2,6,7	      Joystick, IR Remote ,Serial Monitor
2,6,8	      Joystick, IR remote, Bluetooth
2,7,8	      Joystick, Serial Monitor, Bluetooth
3,4,5	      Potentiometer, Button, Rotary encoder
3,4,6	      Potentiometer, Button, IR remote
3,4,7	      Potentiometer, Button, Serial Monitor
3,4,8	      Potentiometer, Button, Bluetooth
3,5,6	      Potentiometer, Rotary Encoder, IR  remote
3,5,7	      Potentiometer, Rotary Encoder, Serial Monitor
3,5,8	      Potentiometer, Rotary Encoder, Bluetooth
3,6,7	      Potentiometer, IR remote, SerialMonitor
3,6,8	      Potentiometer, IR Remote, Bluetooth
3,7,8	      Potentiometer, Serial Monitor, Bluetooth
4,5,6	      Button, Rotary Encoder, IR remote
4,5,7	      Button, Rotary Encoder, Serial Monitor
4,5,8	      Button, Rotary Encoder, Bluetooth
4,6,7	      Button, IR Remote, Serial Monitor
4,6,8	      Button, IR Remote, Bluetooth
4,7,8	      Button, Serial Monitor, Bluetooth
5,6,7	      Rotary Encoder ,Serial Monitor
5,6,8	      Rotary Encoder, IR Remote, Bluetooth
5,7,8	      Rotary Encoder, Serial Monitor, Bluetooth
6,7,8         IR remote, Serial Monitor ,Blue tooth

The Extra combinations (double triple ups)
1,1,1
2,2,2
3,3,3
4,4,4
5,5,5
6,6,6
7,7,7
8,8,8
1,2,2
1,3,3 etc
