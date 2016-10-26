FROM library/debian:jessie
RUN apt-get update && apt-get install git uuid-runtime debootstrap libxml-parser-perl gfxboot zsync cpio --yes
RUN wget http://mirror.thson.de/lernstick/pool/main/l/live-build/live-build_5.0~a5-1%2blernstick2_all.deb && dpkg -i live-build_5.0~a5-1+lernstick2_all.deb
CMD git clone https://github.com/THS-on/lernstickcloud.git /lernstickcloud && cd /lernstickcloud && git checkout jessie32 && ./build_dvd.sh

