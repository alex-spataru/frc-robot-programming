# Robot Components

One of the most important things in programming is that you need to understand what are you programming. If you want to write a game, you need to understand how a game works. If you want to write software for a robot, you need how the robot works.

FRC robots are easy to understand because FIRST enforces a set of standards for all FRC teams. In most cases, you can only use “official” or “approved” hardware for your robot.

There are some exceptions to this rule. For example, you may use "unofficial" sensors to enhance the functionality of your robot. Our 2015 robot uses [Rockwell's VisiSight](http://ab.rockwellautomation.com/Sensors-Switches/Miniature-Photoelectric-Sensors/VisiSight-Photoelectric-Sensors) sensors to avoid jamming the elevator system.

### The RoboRIO

The RoboRIO is one of the most important components of a FRC robot. It’s a computer that loads your robot code automatically and manages the robot components with it.

![RoboRIO with Labels](http://khengineering.github.io/RoboRio/controls/Images/roborio.jpg)

**Its tech specs are**:
-	Dual-core ARM Cortex A9 Processor @ 667 MHz
-	256 MB of RAM 
-	512 MB of Flash memory
-	Supports USB 2.0 and USB 3.0 devices
-	Runs a modified version of the Linux kernel
-	Integrates the Analog I/O, Digital I/O and PWM Control modules into one component

### The Power Distribution Panel (PDP)

The PDP is in charge of sending electrical power to all the robot components. All FRC teams are enforced to use this panel for safety reasons. Every component that requires electricity must be connected to the PDP. If there’s a short on the robot, the PDP will trip the corresponding breaker automatically.

![PDP with Labels](http://khengineering.github.io/RoboRio/controls/Images/pdpinfo.png)

### The Pneumatics Control Module

The pneumatics control module allows you to control the robot's pneumatic components. Its commands run through CAN bus.

![PCM with Labels](http://khengineering.github.io/RoboRio/Images/pcminfo.png)

### The motor controllers

In FRC robots (and most robots), you don't have access to the motor actuators directly. You need to wire your motor to a Talon, Jaguar or Victor controller to control it.

As of May 2015, the allowed motor controllers for FRC teams are:

![Motor Controllers](http://khengineering.github.io/RoboRio/Images/motorcontrollers.png)

The primary differences between the motor controllers above are:

- **Safety**: air intakes posses a serious security threat to your robot. Avoid them when possible.
- **Size**: depending on your robot, you may appreciate the smaller sized motor controllers.
- **Output**: each motor controller has a different way to control a motor. The best way to test this is by plugging in a motor and testing its performance with each controller.
- **Temperature efficiency**: older models, such as the Jaguar and Victor 888 controllers, may take more time to cool down than newer controllers.

Our team prefers to use the Victor SP controllers for secondary subsystems, such as the elevator or rollers. We use the Talon SRX controllers for primary subsystems, such as the drive system.