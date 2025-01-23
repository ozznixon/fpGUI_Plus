# See: https://github.com/graemeg/fpGUI

fpGUI+ information
=================
 This version of fpGUI is based on the original works from Graeme G. My [FORK] includes
 a few code fixes, mainly new additions: fpg_style_luna (+ 7 more). I picked fpGUI as it
 (a) already works, (b) looks the same on my RPi, Mac, Ubuntu, and Win32/64 machines. My
 company and I develop: BOA (Back Office Accounting), Point of Sale, Pawn Shop Manager,
 and many FIDONet and BBS products. It is imparative to have a standardized U/I everywhere
 so we can use the same screenshots in our manuals, website, etc.

To install FPC under Debian/Ubuntu
==================================
 Select the fpc.deb metapackage, which depends on a number of sub-packages
 containing the compiler, the units and so on. The 'libc' unit provided by
 FPC is included in the fp-units-i386.deb package, which is however marked
 as "deprecated" by the Ubuntu package manager and is therefore *not*
 installed by default using fpc.deb.

 The following command will set up FPC under Ubuntu in order to be used with
 fpGUI:

   sudo apt-get install fpc fp-units-i386



How to compile fpGUI
====================
 Please see the INSTALL.txt file for detailed instructions.



System requirements
===================

a) Fonts

If the AggCanvas rendering is enabled, then make sure you have the
Liberation Sans font installed under Linux and FreeBSD. Under Windows,
AggCanvas will use the Arial font, already included with Windows.

b) Linux

To be able to compile and link fpGUI based applications you need to install
the following library dependencies. The packages will pull in all the other
required packages too.

  $ sudo apt-get install libX11-dev
  $ sudo apt-get install libXft-dev

NOTE:
  On some Linux systems (eg: Ubuntu 17.04) those package names are now
  in all lower-case.

    $ sudo apt-get install libx11-dev
    $ sudo apt-get install libxft-dev

c) FreeBSD, OpenSolaris

Pretty much the same as under Linux. Also, if Liberation Sans font is not
available, it can be installed as follows:

  $ pkg install liberation-fonts-ttf



                ============================================
