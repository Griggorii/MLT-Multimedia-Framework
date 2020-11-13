# MLT-Multimedia-Framework
MLT Multimedia Framework recompilation os 20.04 , python3.8 native redirect include

MLT Multimedia inpack mlt-master.tar.xz

sudo apt install dh-python frei0r-plugins-dev gir1.2-gtk-2.0 gir1.2-harfbuzz-0.0 icu-devtools ladspa-sdk libavformat-dev libavutil-dev libblkid-dev libcaca-dev libcairo-script-interpreter2 libcairo2-dev libdatrie-dev libdbus-1-dev libdv4-dev libebur128-dev libegl-dev libegl1-mesa-dev libeigen3-dev libepoxy-dev libexif-dev libexif-doc libexif-gtk-dev libexif-gtk5 libffi-dev libfftw3-bin libfftw3-dev libfftw3-long3 libfftw3-quad3 libfontconfig1-dev libfreetype-dev libfreetype6-dev libfribidi-dev libgdk-pixbuf2.0-dev libgl-dev libgl1-mesa-dev libgles-dev libgles2-mesa-dev libglib2.0-dev libglib2.0-dev-bin libglu1-mesa-dev libglvnd-dev libglx-dev libgraphite2-dev libgtk2.0-dev libharfbuzz-dev libharfbuzz-gobject0 libibus-1.0-dev libice-dev libicu-dev libmount-dev libmovit-dev libmovit8 libpango1.0-dev libpcre16-3 libpcre2-dev libpcre2-posix2 libpcre3-dev libpcre32-3 libpcrecpp0v5 libpixman-1-dev libpng-dev libpng-tools libpopt-dev libpostproc-dev libpthread-stubs0-dev libpulse-dev libpython3-dev libpython3.8-dev libqt5concurrent5 libqt5opengl5 libqt5opengl5-dev libqt5sql5 libqt5sql5-sqlite libqt5svg5-dev libqt5test5 librtaudio-dev librtaudio6 libsamplerate0-dev libsdl1.2-dev libsdl2-dev libselinux1-dev libsepol1-dev libslang2-dev libsm-dev libsndio-dev libsox-dev libsox-fmt-all libsox-fmt-alsa libsox-fmt-ao libsox-fmt-base libsox-fmt-mp3 libsox-fmt-oss libsox-fmt-pulse libsox3 libswresample-dev libswscale-dev libthai-dev libudev-dev libwayland-bin libwayland-dev libx11-dev libxau-dev libxcb-render0-dev libxcb-shm0-dev libxcb1-dev libxcomposite-dev libxcursor-dev libxdamage-dev libxdmcp-dev libxext-dev libxfixes-dev libxft-dev libxi-dev libxinerama-dev libxkbcommon-dev libxml2-dev libxrandr-dev libxrender-dev libxss-dev libxt-dev libxv-dev libxxf86vm-dev pango1.0-tools python3-dev python3.8-dev qt5-qmake qt5-qmake-bin qtbase5-dev qtbase5-dev-tools qtchooser swig swig4.0 uuid-dev x11proto-core-dev x11proto-dev x11proto-input-dev x11proto-randr-dev x11proto-scrnsaver-dev x11proto-xext-dev x11proto-xf86vidmode-dev x11proto-xinerama-dev xorg-sgml-doctools xtrans-dev

in folder mlt-master run terminal command and command dpkg-buildpackage -rfakeroot -b

$ ./configure --build=x86_64-linux-gnu --prefix=/usr --includedir=${prefix}/include --mandir=${prefix}/share/man --infodir=${prefix}/share/info --sysconfdir=/etc --localstatedir=/var --disable-silent-rules --libdir=${prefix}/lib/x86_64-linux-gnu --runstatedir=/run --disable-maintainer-mode --disable-dependency-tracking --enable-gpl --enable-gpl3 --enable-motion_est --enable-mmx --enable-sse --avformat-shared=/usr --swig-languages=python --qimage-libdir=/usr/lib --disable-swfdec

$ make -j16

$ make install


original https://github.com/mltframework/mlt
