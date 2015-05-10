# Robot Components

FRC robots are easy to understand because FIRST enforces a set of standards for all FRC teams. For example, you can only use “official” or “approved” hardware for your robot.

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
