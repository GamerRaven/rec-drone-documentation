# Introduction
After your workshop, you should have worked with Blockly and obtained a general idea of what CoDrone is like. This documentation is intended to guide you through more advanced coding knowledge, and some general tips by old Drones members.

While Blockly is an acceptable coding tool for CoDrone EDU, this documentation is designed for Python and I strongly recommend using it instead.

The objective of coders is to complete the same course flew by pilots but autonomously. This mainly involves coding movement. However, THE MAIN CHALLENGE of coding is to ensure consistency. As you experiment with the code, you would realize the same code segment may produce different results everytime.
``` py title="Sample Move"
from codrone_edu.drone import Drone
drone = Drone()
drone.pair()

drone.move()
drone.set_throttle(50)
drone.move(1)
drone.set_throttle(0)
drone.set_roll(50)
drone.move(1)
drone.land()
```
The code above is intended to move the drone forward and then right. But if you test the code over multiple runs, you would realize that the drone ends up at a different location despite having the same code, starting location, and environment. This is due to several known and unknown factors, but you just need to understand that the drone behaves weirdly. We must rely on sensors, which we will address in this documentation. 

## Python Installation
### Install Python 3.11.6
Visit [https://www.python.org/downloads/release/python-3116](https://www.python.org/downloads/release/python-3116)

### Install PyCharm
Visit [https://www.jetbrains.com/pycharm/download/](https://www.jetbrains.com/pycharm/download/)

Sorry about my fan:
![type:video](https://www.youtube.com/embed/yoxNW6Q9aQY)