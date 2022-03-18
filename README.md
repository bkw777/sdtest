# sdtest
Very basic speed test for a storage device.

Intended for small computers that run from sdcards like Raspberry Pi.  

Tests 4k random read/write for [application performance class 1](https://www.jeffgeerling.com/blog/2019/a2-class-microsd-cards-offer-no-better-performance-raspberry-pi)  
Does the same [sd card speed test](https://www.raspberrypi.com/news/sd-card-speed-test/) as [agnostics](https://github.com/raspberrypi-ui/agnostics), but without needing all the rest of the gui app and gtk & X11 libraries that would get pulled in by installing agnostics.
Requires [fio](https://fio.readthedocs.io/en/latest/index.html) and bash.

More info:
https://github.com/ThomasKaiser/Knowledge/blob/master/articles/A1_and_A2_rated_SD_cards.md  
https://www.tomshardware.com/best-picks/raspberry-pi-microsd-cards  
https://www.jeffgeerling.com/blog/2019/raspberry-pi-microsd-card-performance-comparison-2019

## install
  sudo -i
  apt install fio bash
  curl https://raw.githubusercontent.com/bkw777/sdtest/main/sdtest > /usr/local/bin/sdtest
  chmod 755 /usr/local/bin/sdtest

## usage
  sdtest
