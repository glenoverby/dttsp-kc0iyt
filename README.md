# dttsp
This is a program that implements a Software-Defined Radio

This is a fork of the 'dttsp' respository with changes I have made.

## Changes:
 - beacon-keyer	Sends repeated 0 characters to serve as a beacon
 - text-keyer	Keyboard keyer with an option to take input from a commandline option

## Other Branches:
  - kc0iyt-32k-spec-buckets
	Changes the spectrum data to a signed character, and increases the
	number of spectrum buckets to 32768.  The data + header fits in a
	64kb UDP packet
  - kc0iyt-udp
	I/Q data is transfered over UDP instead of JACK Audio. Includes
	resampling (imported from PowerSDR DttSP library) so that JACK can
	run at 48khz and the UDP data stream can be 192khz.

