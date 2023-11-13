# Movement-of-Robot-Joints
## Aim:  
To move and drive the joints of the robot using python API.

## Equipment’s required:

Visual Components Premium 4.3

## Procedure:

1. 	In the eCatalog panel, Collections view, browse to Models by Type>Robots>Visual Components and then add a Generic Articulated Robot to the 3D world.
2. 	Click the Modeling tab, and then add a Python Script behaviour. The script editor will open automatically when you add the behaviour.
3. 	In the script editor, add the code and then compile the code.

## Program
```
from vcScript import *
from vcHelpers.Robot2 import *
def OnRun():
pos = [[1,30],[2,40],[3,90]]
robot = getRobot()
robot.driveJoints (0,0,0,0,0,0)
delay(5)
for i in pos:
robot.Controller.moveJoint (i[0],i[1])
delay (5)

```
## Output
### 1. Generic Articulated Robot

![image](https://github.com/Preetha-Senthamilan/Movement-of-Robot-Joints/assets/119390282/69a46377-5077-4a02-8129-af1129922e6a)


### 2. robot.driveJoints(0,0,0,0,0,0)

![image](https://github.com/Preetha-Senthamilan/Movement-of-Robot-Joints/assets/119390282/9bd594bc-3404-40df-9579-2a02d4b6a286)


### 3. Movement of Joint1

![image](https://github.com/Preetha-Senthamilan/Movement-of-Robot-Joints/assets/119390282/dd58e9b8-8a62-4176-b475-2135c96e00de)


### 4. Movement of Joint2

![image](https://github.com/Preetha-Senthamilan/Movement-of-Robot-Joints/assets/119390282/541709a6-52e2-4dc0-9a6e-2a212e08440c)


### 5. Movement of Joint3

![image](https://github.com/Preetha-Senthamilan/Movement-of-Robot-Joints/assets/119390282/a0573df0-164c-4fca-9430-0fa4fe6e5ac4)

## Result 

Thus the different robots joints are moved with the help of python list.


