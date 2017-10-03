#Setup
Execute:
To clone the wine source, run:
```git clone git://source.winehq.org/git/wine.git && cd wine```
then, download the patch
```wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch```
apply the patch
```patch -p1 < cuphead.patch```
then start configuring:
```./configure```
and compile:
```make -j5```
and install
```sudo make install prefix=/usr```
#TL;DR
```git clone git://source.winehq.org/git/wine.git && cd wine && wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch && patch -p1 < cuphead.patch && ./configure && make -j5 && sudo make install prefix=/usr```
