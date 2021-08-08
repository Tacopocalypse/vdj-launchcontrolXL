# vdj-launchcontrolXL
Virtual DJ - Controller template for Novation Launch Control XL

Todo:

*Import similar template for adjustment.
*Work with MIDIOX and VDJ developer docs to generate template
*Document in readme, and cleanup.

Use case for this template:
------------------------------------------------------
Initially, this should be setup as a channel mixer.
Secondarily, an effects mixer.
Ancillary, add mode switching to the unit.

This will be an attempt to use the XL 'analog' style controls for channel mixing for volume, and effects.
Since I have a 2 channel mixer, it puts a few limitations on using the extra 2 virtual decks.
I would like to use my launchpad as sampler, and my dj controller for mixing.

The sampler I have does not have 'analog' style control.
The DJ controller I have loses a couple of valuable features when I use all 5 stems.
The additional launchpad I have has a mix of 'analog' style, and digital controls, but incessantly spams midi heartbeats that case issues.


This will be tested with the following components:
------------------------------------------------------
- Virtual DJ 8
- Focusrite 4i4
- Pioneer DDJ-SB3
- Novation Launch Control XL
- Launchpad X


LaunchcontrolXL layout
------------------------------------------------------

Columns
- 8 tracks
    - Each track has 3 'analog' knobs
    - 1 slider
	- 2 buttons

Rows
- User button / Factory button (2 buttons - configured as 1 toggle
- Send Select (2 buttons / up & down arrows on button)
- Track/Device Select (2 buttons / left & right arrows on button)
- Device button
- Mute - Organized with bottom buttons
- Solo - Organized with bottom buttons
- Record Arm - Organized with bottom buttons



The following directories are reference, and not required for deploy:
./img
./example
./manual



Controller Definition & Mapping files for VirtualDJ 8
------------------------------------------------------------------------------------------------------------
Definition

The definition files are standard XML files, and must be installed in the MyDocuments/VirtualDJ/Devices/ folder on PC or /users/YOURNAME/Documents/VirtualDJ/Devices on Mac.

The syntax of the definition file depends on the interface used (HID or MIDI):
Controller Definition syntax for MIDI
Controller Definition syntax for HID


Note : If you wish to build a custom definition for a natively supported Controller, you will need to name the definition file as force-whatevername.xml in order the built-in definition to be bypassed.


Mapping file

The mapping files are also standard XML files, and must be installed in the MyDocuments/VirtualDJ/Mappers/ folder on PC or /users/YOURNAME/Documents/VirtualDJ/Mappers/ on Mac.

Mapping files for the built-in (Native supported) controllers will only appear in this folder if they have been modified by the user via CONFIG -> Mappers in VirtualDJ.
Controller Mapping syntax

------------------------------------------------------------------------------------------------------------


Example XML retrieved from user: PhilW
Discoverd at this link:
http://www.virtualdj.com/forums/227508/VirtualDJ_Plugins/Novation_LaunchControl_XL_Definition_File_and_Mapper.html

Weill use this to kickstart the custom template



Notes:

./img contains images of device and current mapping.
./manual contains dev manual from novation, and any associated manuals from VDJ
./example contains example code for initial guidance


