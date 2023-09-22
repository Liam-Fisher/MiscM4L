# MiscM4L
Miscellaneous M4L devices for Ableton Live. 

MIDI Effects

Seq
Step Sequencer with separable pitch, velocity, and duration cycles. 
Uses a contour | pitch class set (chord) model, so that both can be changed separately to produce the sequence of pitches.  
Input sequences with a midi input device or track, while the corresponding input toggle is on. 


Roll
Step Sequencer with separable pitch, onset, velocity and duration cycles. 
(1-2 voices per note).

Uses the Bach package, which will need to be downloaded in Max. 
There are 4 input options:
Use multisliders and sequence lengths with the number boxes.
Use the bach.roll object as a notation editor (see corresponding documentation),
Use the on/off toggle to record midi input,
Use the "eval" button to input expressions in the Bach "bell" language (see corresponding documentation),
Access the sequences with the variable names + A/B e.g. pitchesA, velocitiesB

Instruments

Gyro_Osc
Requires the gyrosc iphone app, available on the apple store for 99 cents. 
Device for mapping your phone's orientation to Live parameters
change the arguments to the udpreceive object to receive other parameters (like the acceleration vector)



GyroNode
Same as above but uses nodejs to handle udp networking 
much more finnicky, but could be useful as a template for another node based device.

Audio

HRTF (head related transfer function)
Device for controlling spatialization in 3-D

based on a patch by Jakob Hougaard Andersen found at http://jakobhandersen.dk/projects/fft-based-binaural-panner/download/

changed to simplify dsp chain, port to Ableton Live enviroment, and add smoothing functions/hrtf mixing to input data streams

the original license is as follows:

FFT-based binaural panner by Jakob Hougaard Andersen is licensed under a
Creative Commons Attribution 3.0 Unported License: 
https://creativecommons.org/licenses/by/3.0/

The FFT-based binaural panner uses the CIPIC HRTF database which is free to use and redistribute on the terms described at the database website 
https://www.ece.ucdavis.edu/cipic/spatial-sound/hrtf-data/
One of these terms is the inclusion of the database copyright notice: 
'Copyright (c) 2001 The Regents of the University of California. All Rights Reserved'

It is made to be used with Max (by Cycling ’74) which is licensed under its own terms.
