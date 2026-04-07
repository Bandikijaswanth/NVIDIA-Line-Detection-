# NVIDIA-Line-Detection-
AIM

To implement a line-following control rule based on pixel offset.

PROCEDURE
Initialize the pixel offset value
Check the sign of the offset
If offset > 0, robot has drifted right
Command a left turn to correct alignment
Otherwise, adjust accordingly
Display the result
CODE
# Pixel offset
offset = 25   # in pixels

# Line-following logic
if offset > 0:
    action = "Turn Left"
elif offset < 0:
    action = "Turn Right"
else:
    action = "Move Straight"

# Output
print(action)
OUTPUT

Turn Left

RESULT

The robot correctly performs a left turn when a positive offset is detected, ensuring proper line tracking.
