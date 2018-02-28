# ESP32-8266-Sensor-Monitor
AN ESP32/8266 is used to receive sensor data from clients and then log and display the results

A sensor monitor that receives and displays on a webpage client data, usually from an ESP configured as a sensor

Download the files to your IDE location.Locate the files referenced in the Server and Clients, download those and place in your Libraries folderChoose an IP address for your Server e.g. 192.168.0.99

Edit the Server IP address accordingly.

Test the Server by complining and uploading to either an ESP8266 or ESP32, the code adapts accordingly with conditional compile statments. The address of the libraries is included.

Make sure you choose the correct board type!

Test the server by typing this in a browser address bar: http://sensorserver.local/sensor?Sensor=1&temperature=21.2&humidity=50.1&pressure=1001&spare=0&sensortype="Mine"

Or if your PC does not have 'Bonjour' installed, this is needed to resolve mult-cast DNS packets and resolves the address sesnorserver.local to the IP address, in which case enter in the browser address bar:http://192.168.0.99/sensor?Sensor=1&temperature=21.2&humidity=50.1&pressure=1001&spare=0&sensortype="Mine"

For Clients, find the example IP address of 192.168.0.99 and edit this to match your choice of IP address for the Sensor Monitor.

For the Clients, wire your sensors accordingly and change the sensor pins in the Source code to match your pins.

Compile and uploadAdjust the names and types and units as desired.

To see the sensors use http://sensorserver.local/sensor or http://192.168.0.99/sensorTo test the server use http://sensorserver.local/ or http://192.168.0.99/

Upload the example icons to your SD Card using the ESP.
