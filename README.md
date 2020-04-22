# mowZILLA
this is a software and hardware project to "smart UP" a robomower without hardwired connections to the robomowers board, sensors or actuators 

## Robomower hardware

Yardforce 600 ECO
this robomower has no bluetooth, wifi or any other connection to tell if it is 
Workcycle, Mowing, charging, lifted/tilted, ERROR or low on battery
In fact, all of this above mentioned states are indicated via LEDs at the cockpit and some of them followed by a dedicated sound/beep   pattern.

## Environment:
wifi is available for about 50% in the area of our lawn/yard
mowZILLA hardware has to be low power and powerd by battery, since it wont be connected to the robomower's battery or charging station

## Idea:
### Sensing:
use photo electric resistors (sensors) to interpret the LED output lights of the robomowers cockpit
use microphone (sensor) to interpret the indications of the sound/beep patterns.

### Logging:
log all the events on a device

### Connections:
connect to local wifi if available during the different cylces of the robomower

### Reporting / Messaging:
send messages to a recepient 
 - via email
 - via whatsapp
 - other existing message services that can be looked up on any mobile device (android / apple)
