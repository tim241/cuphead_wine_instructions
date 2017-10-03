# Setup
# 1: Clone the wine source <br />
```git clone git://source.winehq.org/git/wine.git && cd wine``` <br />
# 2: Download the patch <br /> 
```wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch``` <br />
# 3: Apply the patch <br /> 
```patch -p1 < cuphead.patch``` <br />
# 4: Configure <br />
```./configure``` <br />
# 5: Compile <br />
```make -j5``` <br />
# 6: Install <br />
```sudo make install prefix=/usr``` <br />
# TL;DR <br />
```git clone git://source.winehq.org/git/wine.git && cd wine && wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch && patch -p1 < cuphead.patch && ./configure && make -j5 && sudo make install prefix=/usr``` <br />
