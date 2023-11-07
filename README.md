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
  pos=[[1,30],[2,40],[3,90]]
  robot = getRobot()
  robot.driveJoints(0,0,0,0,0,0)
  delay(5)
  for i in pos:
    robot.Controller.moveJoint(i[0],i[1])
    delay(5)
```
## Output
### 1. Generic Articulated Robot

![image](https://github.com/Migaleyy/Movement-of-Robot-Joints/assets/118262199/7b45f9c0-8d39-4a04-b295-5b69ce7d4c92)

### 2. robot.driveJoints(0,0,0,0,0,0)

![image](https://github.com/Migaleyy/Movement-of-Robot-Joints/assets/118262199/f7c7c245-47b5-4a2d-8175-ebc6859a6d7f)

### 3. Movement of Joint1

![image](https://github.com/Migaleyy/Movement-of-Robot-Joints/assets/118262199/bfd10c3f-f0ce-4b17-b979-b2809f3ec955)

### 3. Movement of Joint2

![image](https://github.com/Migaleyy/Movement-of-Robot-Joints/assets/118262199/4a6cc883-937c-4b65-943c-5a84c4754c33)

### 3. Movement of Joint3

![image](https://github.com/Migaleyy/Movement-of-Robot-Joints/assets/118262199/ed96168f-a2aa-4536-a5de-2df536021d9d)

## Result 
Thus the different robots joints are moved with the help of python list.


