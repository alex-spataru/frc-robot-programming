# How an FRC Robot Works

FRC robots are relatively easy to understand because FIRST enforces a set of standards that every FRC team needs to follow in order to compete. For example, you can only use a limited set of motor controllers and you may use only “official” or “approved” hardware for your robot.

### The RoboRIO

The RoboRIO is one of the most important components of a FRC robot; it’s a computer that loads your robot code automatically, makes available the Analog, Digital and PWM devices to the programmer and manages every attached device with your code.

![RoboRIO with Labels](http://khengineering.github.io/RoboRio/controls/Images/roborio.jpg)

**Its tech specs are**:
-	Dual-core ARM Cortex A9 Processor @ 667 MHz
-	256 MB of RAM 
-	512 MB of Flash memory
-	Supports USB 2.0 and USB 3.0 devices
-	Runs a modified version of the Linux kernel
-	Integrates the Analog I/O, Digital I/O and PWM Control modules into one component

### The Power Distribution Panel (PDP)

The PDP is in charge of sending electrical power to all the robot components. All FRC teams are enforced to use this panel for safety reasons; every component that requires electricity must be connected to the PDP. If there’s a short on the robot, the PDP will trip the corresponding breaker automatically.

![PDP with Labels](http://khengineering.github.io/RoboRio/controls/Images/pdpinfo.png)

### The Pneumatics Control Module

If your team uses pneumatics to control some aspects of your robot, you will need this module to control your pneumatic components.

![PCM with Labels](http://khengineering.github.io/RoboRio/Images/pcminfo.png)
