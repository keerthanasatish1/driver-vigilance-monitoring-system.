# driver-vigilance-monitoring-system.
The proposed system detects the driver drowsiness using estimation method which
is purely MATLAB based. Here a camera keeps monitoring the driver’s eye every now and
then. If the eyes is closed for duration of time, it alerts the system that the driver is under
drowsiness and this condition is supposed to be the worst case scenario.

The camera first captures the face of the driver then using MATLAB code the driver
eye part is extracted to detect whether the driver is drowsy or not and the steps to extract the
driver eye part is as follows.
 Step 1: Initialize the camera in by using Matlab command.
 Step 2: Take snapshots of the driver (4 to 5) using Matlab command.
 Step 3: Write the MATLAB command to extract face part.
 Step 4: Then remove the edges in the face by estimation method
 Step 5: Extract the eye
 Step 6: Convert gray image into binary image applying canny edge detection.
 Step 7:Calculate the distance for each image and compare with the threshold
values.
 Repeat the procedure for all images.Calulate the percentage of eye
closure.depending on the percentage decide whether the driver is sleepy or awake.
 Step 8: Initialize the serial communication to send the data. Then microcontroller
receives the data via max232, and display the message on LCD based on the
message received Alarm is activated if driver is drowsy, then we send this data via
zigbee to receiver.
 Step 9: Then another zigbee is used for the reception at the receiver section to
send the data to the microcontroller which drives alarm and LCD again.
