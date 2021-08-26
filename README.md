# LaserHarp
Contains code and project files for the Laser Harp project

The Laser harp project accepts inputs from the laser sensors/beams. When a laser beam is interrupted, the consequent signal will be converted into a musical/audio output corresponding with the 'string' played. As such, this functions generally as a classical harp, simply implementing the lasers to operate as harp strings.

Currently the project is controlled by a teensy with an audio shield. The 5 volt power source is stepped down to 3.3 volts to power 8 always on lasers which are pointed at photodiodes. The photodiodes each have a simple BJT circuit to amplify their output which is detected by the teensy. The audio shield on the teensy generates a tone every time a laser beam is interrupted.

The original board schematic is handwritten in LaserHarpSchematic.pdf, but the new schematics and layouts are in the .sch and .brd files respectively.
