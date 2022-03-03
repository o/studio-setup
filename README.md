## Studio setup

I am using this repository as online documentation of my DAW-less (no-computer) setup.

The setup consists of several devices including:

* [Squarp Pyramid MK3](https://squarp.net/pyramid/) Main sequencer and clock source
* [Akai Pro MPC One](https://www.akaipro.com/mpc-one) Sampler / Sequencer 
* [Access Virus TI2](https://www.virus.info/virusti/overview) Digital Synthesizer
* [Moog Subsequent 37](https://www.moogmusic.com/products/subsequent-37) Analog Synthesizer 
* [Behringer TD-3](https://www.behringer.com/product.html?modelCode=P0DTD) Analog Bass Line Synthesizer
* [Apple iPad Pro M1](https://www.apple.com/ipad-pro/) Tablet computer

## MIDI

The MIDI routing schema can be found in the [midi-chart.txt](https://github.com/o/studio-setup/blob/master/midi-chart.txt) file.

## Squarp Pyramid Definition files

Squarp Pyramid supports [definition files](https://squarp.net/pyramid/manual/definitionfiles/) for quickly mapping and accessing the connected devices. The definition files related to the current setup can be found under [pyramid-definition-files](https://github.com/o/studio-setup/tree/master/pyramid-definition-files) folder.

## Notes

In the Squarp Pyramid Midi Out settings:

	MIDI A MODE: MIDI OUT
	MIDI A SYNC: SEND
	MIDI B MODE: MIDI OUT
	MIDI B SYNC: SEND

In the MPC ONE:

For the MIDI clock:

	Preferences > MIDI / Sync > Sync Receive - Receive: MIDI Clock
	Preferences > MIDI / Sync > Sync Send - Send: MIDI Clock

Misc

	Preferences > Audio Recording > Recording Bit Depth: 24
	Preferences > Sequencer > Recording - Rec Arm: Multi
