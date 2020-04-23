# DRAFT
# States
this file is setup to document the multiple states the robomower can have and evaluate the indication LEDs. The goal of this evaluation is a valid block diagram in order to to be able to design a state machine. The main status are as follows:
 - docked to charging station
 - docked to charging station (LOCKED)
 - mowing / in operation
 - stopped operation / self
 - Manual STOP
 - Return to charging station

The Iidication LEDs are going to be observed during the different states

<img src=https://github.com/weinzmi/mowZILLA/blob/master/images/Cockpit_schematic_.zone1_indicatorsPNG.PNG width="240">
[Tilt] - [Signal] - [Batery] - [Charge]


## docked to charging station

| LED     | flashing                  | ON               | OFF  | 
|---------|---------------------------|------------------|-----|
| Tilt    |                           |                  |     |
| Signal  | OK                        | no power supply; wire break  |  ?  |
| Batery  |                           |                  |     |
| Charge  | In the process of charging| finidhed charging| no power supply|

## docked to charging station (LOCKED)

| LED     | flashing                  | ON               | OFF  | 
|---------|---------------------------|------------------|-----|
| Tilt    |                           |                  |     |
| Signal  | OK                        | no power supply; wire break  |  ?  |
| Batery  |                           |                  |     |
| Charge  | In the process of charging| finidhed charging| no power supply|

## mowing / in operation

| LED     | flashing                  | ON               | OFF  | 
|---------|---------------------------|------------------|-----|
| Tilt    |         N.A               |         N.A      |  OK |
| Signal  | ?                         | outside of range; no power supply; wire break | OK  |
| Batery  | low battery               |    ??            | OK  |
| Charge  | N.A.                      | N.A.             | OK  |


## stopped operation / self

| LED     | flashing                  | ON               | OFF  | 
|---------|---------------------------|------------------|-----|
| Tilt    |                           |                  |     |
| Signal  |                           |                  |     |
| Batery  |                           |                  |     |
| Charge  | N.A.                      | N.A.             | OK  |

## Manual STOP

| LED     | flashing                  | ON               | OFF  | 
|---------|---------------------------|------------------|-----|
| Tilt    |                           |                  |     |
| Signal  |                           |                  |     |
| Batery  |                           |                  |     |
| Charge  | N.A.                      | N.A.             | OK  |

## Return to charging station

| LED     | flashing                  | ON               | OFF  | 
|---------|---------------------------|------------------|-----|
| Tilt    |                           |                  |     |
| Signal  |                           |                  |     |
| Batery  |                           |                  |     |
| Charge  |                           |                  |     |



