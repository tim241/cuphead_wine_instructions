# NOTE: this issue is fixed in wine-staging!
# NOTE: this isn't required anymore!
<br />
<br />
<br />

# Setup
# Execute required command for the platform before compiling
* Linux  <br />
```export prefix=/usr```  <br />
* Mac  <br />
```export prefix=/usr/local```  <br />
# Clone the wine source <br />
```git clone git://source.winehq.org/git/wine.git && cd wine``` <br />
# Download the patch <br /> 
```wget https://raw.githubusercontent.com/tim241/cuphead_wine_instructions/master/cuphead.patch``` <br />
# Apply the patch <br /> 
```patch -p1 < cuphead.patch``` <br />
# 32 bit
* Configure for 32-bit <br />
```./configure``` <br />
* Compile <br />
```make -j5``` <br />
# 64 bit with 32 bit support  <br />
* Execute these commands  <br />
```mkdir ../win32```  <br />
```mkdir ../win64```  <br />
```cd ../win64```  <br />
* Configure and make the 64 bit build  <br />
```../wine/configure --with-x --enable-win64 --with-gstreamer && make -j5```  <br />
* Install the 64 bit build  <br />
```sudo make install prefix=$prefix dlldir=$prefix/lib/wine libdir=$prefix/lib```  <br />
* cd into the 32 bit build directory  <br />
```cd ../win32```  <br />
* Configure and make the 32 bit build with 64 bit support  <br />
```../wine/configure --with-x --with-wine64=`pwd`/../win64 --libdir=$prefix/lib32 && make -j5```  <br />
* Install the 32 bit wine with 64 bit support  <br />
```sudo make install prefix=$prefix libdir=$prefix/lib32 dlldir=$prefix/lib32/wine```  <br />


# Install <br />
```sudo make install prefix=$prefix``` <br />
# Uninstall <br />
```sudo make uninstall prefix=$prefix```<br />

