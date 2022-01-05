# qt_teleop
Package for controlling the arms and head of QTrobot with a joypad

## Control
* Left button - activates left arm
* Right button - activates right arm
* Right and left buttons at once - activate head
* Left mini-stick - in case of:
  * arm - changes shoulder pitch (stick y-axis) and shoulder roll (stick x-axis) angles,
  * head - changes head pitch (stick y-axis) and head yaw (stick x-axis) angles
* Right mini-stick - in case the arm is activated, changes elbow roll angle (stick x-axis)
* Four action buttons execute the following actions:
  * A - send kiss
  * B - clapping
  * X - hi
  * Y - one arm up
