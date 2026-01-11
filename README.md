# random-movement-lockon
Lock-on method for randomly moving object.
This code is realisation of my mathematical model of upgraded version of PID regulator from control theory, which developed as an idea for an anti air defence machine.
Key idea is the following:
PID control can only be used if the target location (in our case the state is location, not necesseraly the case in every system ex. temperature, humidity etc. can be measured) is known, when the location is unknown PID regulator is useless.
If instead of using one measuring device but rather two of them with their measuring range intersecting partly at the center, such system could capture the information if the running target by dissapearing from sight left the area by leaving first the center
afterwards being in the measuring range of either one of the devices only then finally dissapearing from sight completely.

Ex1:

  left    center   right
|--------|======|--------|


This information is crucial if it is our goal to catch the target as soon as possible when it left, now with this system it is known to which side the target left and the system can rapidly accerelate in that direction without randomly scanning the area again
in search of the target.
