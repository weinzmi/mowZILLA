# mowZILLA
this is a software and hardware project to "smart UP" a robomower without hardwired connections to the robomowers board, sensors or actuators 

## Robomower hardware

Yardforce 600 ECO
this robomower has no bluetooth, wifi or any other connection to tell if it is 
Workcycle, Mowing, charging, lifted/tilted, ERROR or low on battery
In fact, all of this above mentioned states are indicated via LEDs at the cockpit and some of them followed by a dedicated sound/beep   pattern.

### Cockpit
overview of the buttons and indicator LEDs

<img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_schematic_zones.PNG width="300">

it is devided into 5 zones / funtional areas

<img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_schematic_zones.PNG width="300">

 - Zone 1: LED indicators for the machine status
 - Zone 2: Working time setting area
 - Zone 3: Signal setting
 - Zone 4: Locking button
 - Zone 5: Home & Start button.

Focus area is zone 1 with it's indicator LEDs

<img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_schematic_.zone1_indicatorsPNG.PNG width="300">

this LEDs indicate the following status

 - Tilt - Your mower has been lifted during use for some reason
 <img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_ICON_tilt.PNG width="60">
 
 - Signal - The mower cannot receive the signal sent from the boundary wire
 <img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_ICON_signal.PNG width="60">
 
 - Battery - Battery voltage is too low to perform normal mowing
 <img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_ICON_battery.PNG width="60">
 
 - Charge - In the process of charging
 <img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_ICON_charge.PNG width="60">
 
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
