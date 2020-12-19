# portaudio-pulse
PortAudio with PulseAudio low-level library

See original works here: https://github.com/illuusio/assembla-mirror-portaudio-pulseaudio/tree/PulseAudioHostAPI

Step to build this library:

$ sudo apt-get install pulseaudio libpulse-dev

$ sudo apt-get install automake

$ sudo apt-get install libtool

$ cd portaudio-pulse

$ sudo chmod a+x configure

$ aclocal

$ libtoolize -f

$ autoconf -f

$ automake -f

$ ./configure --with-pulseaudio --without-alsa --without-oss --without-jack

$ make

$ sudo make install

Sometimes additional step needed:

$ sudo ldconfig

$ export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/local/lib
