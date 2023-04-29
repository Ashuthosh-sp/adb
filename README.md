# adb
This is a ADB Driver that is used to establish connection betwween phone and PC..
To Run this .exe file,make sure that the Desktop Folder is present in the User's folder . If not, create a folder called Desktop and then install the ADB exe file
Then go the the local disk c where the ADB is installed and open the command prompt in that  particular location.
Connect the phone to the PC through USB and make sure the phone has USB Debbugging enabled.
Then in the command prompt type the command "adb devices" so that it can list all the devices.
Next run the command  "adb reverse tcp:<destination_port> tcp:<source:port>" where destination port is the port of the phone where it has to be opened (say localhost:4200)
and source port is the port which is active in the PC(say localhost:3000)
Eg: adb reverse tcp:4200 tcp:3000
minimize the command prompt and run the localhost port on the phone which was specifed.
