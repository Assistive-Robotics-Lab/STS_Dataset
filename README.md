# STS_Dataset
Sit-to-stand data from xsens suit, balance board and seating mat from 25 healthy and 6 stroke participants. 

Created by Tom Bennett and Virginia Ruiz Garate, 2022. 

Reference this dataset using the accompanying DOI if you use it in your own research.

### 31 zip folders containing data for individual users, each comprising of: 

  * Raw Files - 4 trials of 5xSTS for each sensor.
  
  * Split files - within Sit_to_stand or Stand_to_sit folders, then within 100% or 115% seat height folders - 10 actions for each sensor.
  
  * Cropped split files - alongside Split files, but cropped to only include participant's movement.
  
  
 
### XSens Suit data:

Columns for ROS time, then XYZ position and XYZW orientation in quaterion form for 22 body areas. List of which sensors represent which body part:

0) Pelvis
1) L5
2) L3
3) T12
4) T8
5) Neck
6) Head
7) R Shoulder
8) R Upper Arm
9) R Forearm
10) R Hand
11) L Shoulder
12) L Upper Arm
13) L Forearm
14) L Hand
15) R Upper Leg
16) R Lower Leg
17) R Foot
18) R Toe
19) L Upper Leg
20) L Lower Leg
21) L Foot
22) L Toe



### Balance Board
Columns contain Header (timestamp), then Front_left, Front_Right, Rear_Left, Rear_Right, as seen from the participant standing on the board's perspective.


### Seating mat
Columns contain Header (timestamp), then numbers 0 through 255. each row can be reshaped into a 16X16 array, giving the true arrangement of sensors in the mat. ie, cols 0-15 inclusive represent the top row of sensors, 16-31 the second row etc.


## Notes
Some participant folders contain a Notes.txt file. This indicated whether any of the trials failed to record properly, and have been removed. 
