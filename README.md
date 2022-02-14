## Studio setup

I am using this repository as an online documentation of my DAW-less (no-computer) setup.

The setup consists of several devices including:

* [Squarp Pyramid MK3](https://squarp.net/pyramid/) Main sequencer and clock source
* [Elektron Digitakt](https://www.elektron.se/products/digitakt/) Sampler / Drum machine 
* [Access Virus TI2](https://www.virus.info/virusti/overview) Digital Synthesizer
* [Moog Subsequent 37](https://www.moogmusic.com/products/subsequent-37) Analog Synthesizer 
* [Behringer TD-3](https://www.behringer.com/product.html?modelCode=P0DTD) Analog Bass Line Synthesizer
* [Apple iPad Pro M1](https://www.apple.com/ipad-pro/) Tablet computer

## MIDI

The MIDI routing schema can be found in the [midi-chart.txt](https://github.com/o/studio-setup/blob/master/midi-chart.txt) file.

## Squarp Pyramid Definition files

Squarp Pyramid supports [definition files](https://squarp.net/pyramid/manual/definitionfiles/) for quickly mapping and accessing to the connected devices. The definition files related to the current setup can be found under [pyramid-definition-files](https://github.com/o/studio-setup/tree/master/pyramid-definition-files) folder.

## Notes

In the Squarp Pyramid Midi Out settings:

	MIDI A MODE: MIDI OUT
	MIDI A SYNC: SEND
	MIDI B MODE: MIDI OUT
	MIDI B SYNC: SEND

In the Digitakt Midi Config:

	CLOCK SEND: ENABLED
	TRANSPORT SEND: ENABLED

In the Digitakt Channels Config:

	TRACK A CHANNEL: 9
	TRACK B CHANNEL: 10
	FX CONTROL CHANNEL: OFF
	AUTO CHANNEL: OFF

In the main screen: 

* Switch to track 9 and enable CHAN, choose 9
* Switch to track 10 and enable CHAN, choose 10
