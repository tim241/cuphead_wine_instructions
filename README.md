# Setup
Execute: <br />
To clone the wine source, run: <br />
```git clone git://source.winehq.org/git/wine.git && cd wine``` <br />
then, download the patch <br /> 
```wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch``` <br />
apply the patch <br /> 
```patch -p1 < cuphead.patch``` <br />
then start configuring: <br />
```./configure``` <br />
and compile: <br />
```make -j5``` <br />
and install <br />
```sudo make install prefix=/usr``` <br />
# TL;DR <br />
```git clone git://source.winehq.org/git/wine.git && cd wine && wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch && patch -p1 < cuphead.patch && ./configure && make -j5 && sudo make install prefix=/usr``` <br />
