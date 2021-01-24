
# Saponification Damage

## 1-Lead
cutaway, lijantropique 

## 2-Short description
After successfully accessing the OT, the attacker is ready to attack the saponification reactor. The objective is equipment damage (T0879), or at least, affect the product quality to increase production/manufacturing costs (T0828). To accomplish this the attacker would send rogue commands to the PLC to modify set points:

1- Reduce reactor level below Low-Low (would need to disable/change alarm levels before)
2- Close inlet/outlets to trap fluid/gas inside the reactor
3- Open steam valve 100% to increase temperature

The idea is to increase vaporize any trapped liquid and increase pressure beyond design limits. Issue would be physical protections (Safety relief valves or rupture discs), that should pop open in case of over pressure. The history could say that the attacker review the maintenance history and noticed the team is behind checking safety valves (common in some plants), and past test indicated the valve was stuck and never replaced.  


## 3-Exploit Path
Start at Stage 2 (ICS Attack) -> advanced beyond initial access and C2

Inhibit Response Function: Alarm Suppression, Modify Alarm Settings
Impair Process Control: Modify Control Logic
Impact: Damage to Property, Loss of Safety, Loss of Productivity and Revenue


## 4-Requirements
To play this scenario the player should have successfully reach the Control Network either by playing the initial access scenario or because access was given (e.g., part of the read team engagement).
At some point during previous missions, the player must have accessed the engineering workstation to exfiltrate design information and PLC logic.

Finally, the player should have completed the scenario dealing with Process control modification.


## 5-Characters
Red teamer
Professional
(maybe too much resources required for a common criminal)

## 6-Attached Documents
BFD,PFD
Reactor datasheet
Maintenance logs
ladder logic?


## 7-Notes
