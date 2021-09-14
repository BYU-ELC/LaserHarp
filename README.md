# LaserHarp
Contains code and project files for the Laser Harp project

The Laser harp project accepts inputs from the laser sensors/beams. When a laser beam is interrupted, the consequent signal will be converted into a musical/audio output corresponding with the 'string' played. As such, this functions generally as a classical harp, simply implementing the lasers to operate as harp strings.

Currently the project is controlled by a teensy with an audio shield. The 5 volt power source is stepped down to 3.3 volts to power 8 always on lasers which are pointed at photodiodes. The photodiodes each have a simple BJT circuit to amplify their output which is detected by the teensy. The audio shield on the teensy generates a tone every time a laser beam is interrupted.

The original board schematic is handwritten in LaserHarpSchematic.pdf, but the new schematics and layouts are in the Laser Harp PCB.sch and Laser Harp PCB.brd files respectively. You should use these for future development or repair.


FUTURE DEVELOPMENT

Currently the Laser Harp is using a PCB we milled out here in the shop which is nice, but it might be nice to order a professional one. Also, it is Revision 2, meaning I had to manually change the connection from pin 7 to pin 8 (See schematic commit notes).

If the Photo Diode boards are ever replaced, you should add an additional pad to the board to make it easier to connect the power supply since it runs from one board to the next.

It might be nicer to have the buttons attached to the Laser Harp PCB instead of on a separate board, or at least mounted on the base of the Laser Harp more professionally.

The fog currently works, but it could be improved by replacing the fans on the reservoir with stronger fans and possibly redoing the tubing to get better fog distribution.

If someone can find a library of actual harp audio files (instead of piano), that would be awesome. Just make sure to format the files as described the in the Laser Harp Hardware Documentation.
