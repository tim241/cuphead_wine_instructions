# Setup
# Clone the wine source <br />
```git clone git://source.winehq.org/git/wine.git && cd wine``` <br />
# Download the patch <br /> 
```wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch``` <br />
# Apply the patch <br /> 
```patch -p1 < cuphead.patch``` <br />
# Configure
* Configure for 32-bit <br />
```./configure``` <br />
* Configure for 64-bit <br />
```./configure --enable-win64``` <br />
# Compile <br />
```make -j5``` <br />
# Linux
* Install <br />
```sudo make install prefix=/usr``` <br />
* Uninstall <br />
```sudo make uninstall prefix=/usr``` <br />
# Mac
* Install <br />
```sudo make install prefix=/usr/local``` <br />
* Uninstall <br />
```sudo make uninstall prefix=/usr/local``` <br />

