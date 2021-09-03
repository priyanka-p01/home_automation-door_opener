# Home Automation - Smart Door Opener
Code for my personal project of Home Automation - Smart Door opener. The project is simulated on Tinker CAD. Links given in the Readme file!

PROJECT ON TINKER-CAD: https://www.hackster.io/priyanka_p1/home-automation-automated-entrance-exit-door-0d6a22

Story<br>
<b>
Introduction:
 </b>

For long, I have seen and wondered about Home Automation Systems. A lot of projects exist online on how to build smart home automation systems for light intensity, burglar intrusions, voice assistants etc. However, there are very few projects which have a smart home door. Mine belongs to the same category, but is a bit different

A door that opens when it senses motion, and closes when the motion is no longer there. It also opens automatically and rings an alarm / buzzer when the system detects smoke or unwanted gases. How cool does that sound? Well, it is fun to make the project. In this article I will be sharing it.

<b>
Setup & Procedure:
</b>

The system is made as a compact and mobile device. It can be placed over the top the entrance or on the top most part of the door, for better functionality. The hardware used in the system is mentioned in the components part. Here it is shown as connected to the power source via a USB Cable. However, we could independently power it, using Lithium batteries. It might turn out to be a bit expensive, but would be totally worth it.

Let us discuss how the project works:

![image](https://user-images.githubusercontent.com/78416066/131888443-81df8aa3-fb13-4b52-a888-3e62fa963451.png)

When a person stands or approaches the door, about 50 cms away from the door, the Ultrasonic Sensor gets activated due to movement in its range. The PIR sensor also acting as a backup here, keeps the door open until the movement stops. If there is no movement in the given then it closes the door, without the intervention of the Ultrasonic sensor. At the moment, when the door opens, the buzzer just rings for a second signaling that people / objects are passing from the area.

The temperature sensor, here acts like a fire-preventive mechanism. If, due to some fire, there is a huge increase in the room temperature, then it again signals the servo motor to open the door. The last application is about the Gas Detection sensor.

While the servo motor, PIR motion sensor and the Ultrasonic sensor are integrated with the digital input pins of the Arduino board, the Gas detection sensor is connected to Analog input pin of the Arduino. When the value is more than 350, it signals the servo motor to push open the door. It also rings the buzzer in periodic cycles to alarm the people in the room. The door, will automatically close when the PIR / Ultrasonic sensor will fail to detect any movement in their range.
