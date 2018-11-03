
Repository for ubuntu 18.04 desktop changes

Additional installation packages:


Make Line out default audio output:

pactl list short sinks
set-default-sink alsa_output.pci-0000_00_1b.0.analog-stereo

sudo gedit /etc/pulse/default.pa
### Make some devices default
set-default-sink 5
#set-default-source input
