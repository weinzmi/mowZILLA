# mowZILLA
## Summary:
this is a software and hardware project to "smart UP" a robomower without using hardwired connections to the robomowers board, sensors or actuators. Just read information from LEDs and Sound / Bussers to log the condition of the robomower and notify the owner about status changes and actions to be carried out.

### what it is not:
a way to control or change parameters of the robomower

## Robomower hardware

Yardforce 600 ECO
this robomower has no bluetooth, wifi or any other connection to tell it's current state, e.g.:
 - Mowing
 - Charging
 - Lifted/tilted
 - ERROR
 - Low  battery
 
In fact, all of this above mentioned states are indicated via LEDs at the cockpit and some of them are followed by a dedicated sound/beep pattern.

<img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Robomower_yardforce_600_eco.PNG width="300">

here the link to the user manual:
https://www.yardforce-tools.com/ProductFiles/fa4b8085-5971-479d-b8ae-45d6835b5a5c.pdf

### Cockpit
overview of the buttons and indicator LEDs

<img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_schematic_zones.PNG width="300">

The cockpit is devided into 5 zones / funtional areas

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

### Condition Monitoring Information:
some basic calculations based on status changes, durations, tima of day, or other environmental data / information. These information should then be posted in notifications to the end user to take emidiate actions if necessarry or for the purpose of analysis and further optimization.

### Notifications:
send messages to a recepient 
 - via email
 - via whatsapp
 - other existing message services that can be looked up on any mobile device (android / apple)
 
 Notifications should include:
  - Date & Time
  - Category
   - Normal, Warning, ERROR
  - Change of status; from OLD to NEW
  - Actionable information
   - suggestions of actions to be carried out, e.g.:
