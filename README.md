## Studio setup

I am using this repository as an online documentation of my DAW-less (no-computer) setup.

The setup consists of several devices including:

* [Squarp Pyramid MK3](https://squarp.net/pyramid/) Main sequencer and clock source
* [Akai Pro MPC One](https://www.akaipro.com/mpc-one) Sampler and Sequencer
* [Access Virus TI2](https://www.virus.info/virusti/overview) VA Polyphonic Digital Synthesizer
* [Moog Subsequent 37](https://www.moogmusic.com/products/subsequent-37) Paraphonic Analog Synthesizer 
* [Behringer TD-3](https://www.behringer.com/product.html?modelCode=P0DTD) Analog Bass Line Synthesizer
* [Roland SPX-SX](https://www.roland.com/global/products/spd-sx/) Sampling Pad
* [Apple iPad Pro M1](https://www.apple.com/ipad-pro/) Tablet computer used for step sequencing
* [Arturia KeyStep](https://www.arturia.com/keystep/overview) MIDI keyboard with step sequencing
* [Arturia KeyLab 61](https://www.arturia.com/products/hybrid-synths/keylab61/overview) MIDI keyboard

## MIDI Scheme

                  ┌────────────────────────────────────────────────────────────────────────────────────────────────────┐
                  │                                                                                                    │
                  │    ┌────────────────────────────────────────────────────┐                                          │
                  │    │                                                    │                                          │
                  │    ▼                                                    │                                          ▼
        ┌─────────┴─────────────────┐      ┌──────────────────────┐      ┌──┴──────────────┐      ┌────────────────────────────────────────────┐      ┌────────────────────┐      ┌────────────────────────────────┐
        │       THRU  IN 1-16       │      │                      │      │  B              │      │                  IN 15               OUT 16├─────►│IN 16               ├─────►│ IN 14                          │
        │                           │      │               IN 1-16├──────┤A                │      │                                            │      │                    │      │                                │
        │  Access Virus TI 2        │      │  Akai MPC One        │      │  Squarp Pyramid │      │  Moog Subsequent 37                        │      │  Behringer TD-3    │      │  Roland SPX-SX                 │
        │  16 CH                    │      │  128 CH              │      │  64 CH          │      │  1 CH                                      │      │  1 CH              │      │  1 CH                          │
        │                           │      │                      │      │                 │      │                                            │      └────────────────────┘      │                                │
        │                           │      │                      │      │                 │      │                                            │                                  │                                │
        └───────────────────────────┘      │                      │      │                 │      │                                            │                                  │                                │
                                           │                      │      │USB IN      IN   │      │                                            │                                  │                                │
                                           │                      │      └─────────────────┘      │                                            │                                  │                                │
                                           │                      │         ▲          ▲          │                                            │                                  │                                │
                                           │                      │         │          │          │                                            │                                  │                                │
                                           └──────────────────────┘         │          │          └────────────────────────────────────────────┘                                  │                                │
                                                                            │          │                                                                                          │                                │
                                                                            │          │                                                                                          │                                │
                                                                            │          │                                                                                          │                                │
                                                                            │          │                                                                                          └────────────────────────────────┘
                                                                            │          │
                                                       ┌────────────────────┴─┐      ┌─┴─────────────────────────────────────────┐
                                                       │               USB OUT│      │OUT                                        │
                                                       │                      │      │                                           │
                                                       │  iPad Pro M1         │      │  Arturia Keystep                          │
                                                       │                      │      │                                           │
                                                       │                      │      │                                           │  ┌──────────────────────────────────────────────────────────────────────────────┐
                                                       │                      │      └───────────────────────────────────────────┘  │                                                                              │
                                                       │                      │                                                     │                                                                              │
                                                       │                      │                                                     │  Arturia Keylab 61                                                           │
                                                       │                      │                                                     │                                                                              │
                                                       │                      │                                                     │                                                                              │
                                                       │                      │                                                     │                                                                              │
                                                       └──────────────────────┘                                                     └──────────────────────────────────────────────────────────────────────────────┘


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
