## Studio setup

I am using this repository as an online documentation of my DAW-less (no-computer) setup.

The setup consists of several devices including:

* [Squarp Hapax](https://squarp.net/hapax/) Main sequencer and clock source
* [Squarp Pyramid MK3](https://squarp.net/pyramid/) MIDI Sequencer
* [Akai Pro MPC One](https://www.akaipro.com/mpc-one) Sampler and Sequencer
* [Access Virus TI2](https://www.virus.info/virusti/overview) VA Polyphonic Digital Synthesizer
* [Access Virus TI Polar](https://www.virus.info/virusti/overview) VA Polyphonic Digital Synthesizer
* [Moog Subsequent 37](https://www.moogmusic.com/products/subsequent-37) Paraphonic Analog Synthesizer 
* [Behringer TD-3](https://www.behringer.com/product.html?modelCode=P0DTD) Analog Bass Line Synthesizer
* [Roland SPX-SX](https://www.roland.com/global/products/spd-sx/) Sampling Pad
* [Apple iPad Pro M1](https://www.apple.com/ipad-pro/) Tablet computer used for step sequencing
* [Arturia KeyStep](https://www.arturia.com/keystep/overview) MIDI keyboard with step sequencing
* [Arturia KeyLab 61](https://www.arturia.com/products/hybrid-synths/keylab61/overview) MIDI keyboard
* [Tascam Model 12](https://www.tascam.eu/en/model12) Mixer with MIDI transport and multitrack recording

## MIDI Scheme



        ┌───────────────────────────────────────────────────────────────────┐                                                                                  
        │                                                                   │                                                                                  
        │                                                                   │                                               ┌─────────────────┐                
        │                                                                   │      ┌─────────────────────────────────┐      │                 │                
        │        Arturia Keylab 61                                          │      │                                 │      │                 │                
        │                                                                   │      │                                 │      │   Squarp        │                
        │                                                                   ┼─────►│    Arturia Keystep              ┼─────►│   Pyramid       │                
        │                                                                   │      │                                 │      │                 │                
        └───────────────────────────────────────────────────────────────────┘      └─────────────────────────────────┘      └────┬────────────┘                
                                                                                                                                 │                             
                                                                                                                                 │                             
                                                                                                                                 │                             
                                                                                                                                 │                             
                                                                                                                                 │                             
                                                           ┌────────────────────────────────────┐                                │                             
                                                           │                                    │                                │                             
                                                           │                                    │◄───────────────────────────────┘                             
                                                           │                                    │                                                              
                                                           │     Squarp Hapax                   │                                                              
                                                           │                                    │                                                              
                                                           │                                    ┼────────────────────────────────────┐                         
                                                           │                                    ┼──────┐                             │                         
                                                           └─┬─┬────────────────────────────────┘      │                             │                         
                                                             │ │                                       │                             │                         
                                                             │ │                                       │                             │                         
                                                             │ │                                       │                             │                         
                                                             │ │                                       │                             │                         
         ┌────────────────────────────────────┐              │ │                                       │                             │                         
         │                                    │◄─────────────┘ │                                       │                             │                         
         │                                    │                ▼                                       ▼                             │                         
         │                                    │      ┌────────────────────────────────────────┐      ┌──────────────────────┐        │                         
         │                                    │      │                                        │      │                      │        │                         
         │                                    │      │                                        │      │                      │        ▼                         
         │                                    │      │                                        │      │                      │      ┌──────────────────────────┐
         │                                    │      │                                        │      │                      │      │                          │
         │                                    │      │                                        │      │                      │      │                          │
         │                                    │      │                                        │      │                      │      │                          │
         │      Access Virus TI Polar         │      │      Moog Subsequent 37                │      │    Akai MPC One      │      │    Access Virus TI2      │
         │                                    │      │                                        │      │                      │      │                          │
         │                                    │      │                                        │      │                      │      │                          │
         │                                    │      │                                        │      │                      │      │                          │
         └────────────────────────────────────┘      └────────────────────────────────────────┘      └──────────────────────┘      └──────────────────────────┘

TD3 and SPD-SX are not connected via MIDI. I might want to send MIDI from SPD-SX in the future for recording drums.

## Squarp Pyramid Definition files

Squarp Pyramid and Hapax support definition files for quickly mapping and accessing connected devices. These files, related to the current setup, can be found in the respective folders. Since Hapax is used as a main sequencer, I’ll only be updating these definition files.


## Notes

In the Squarp Hapax (for all 4 MIDI Out ports) settings:

	MIDI X MODE: MIDI OUT
	MIDI X SYNC: SEND

In the MPC ONE:

For the MIDI clock:

	Preferences > MIDI / Sync > Sync Receive - Receive: MIDI Clock
	Preferences > MIDI / Sync > Sync Send - Send: MIDI Clock

Misc

	Preferences > Audio Recording > Recording Bit Depth: 24
	Preferences > Sequencer > Recording - Rec Arm: Multi
