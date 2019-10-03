# mglOcm
rom file loader for 1chipMSX(KdL firmware machine) 


mglOCM is a MSX ROM loader for the  "KdL firmware's OneChip MSX"
 that allows you to run msx rom cartridge images (like Konami-SCC, ASCII-8 and ASCII-16, 8, 16, 32k, linear rom files)
 on your device without setting any DIP switches or mapper patches.

Rom Loader for 1Chip MSX - mglOCM v2.0370b (release date 2019/04/12)

v2.0370b :

ABOUT

- This is the loader application that support to execute megarom cartridge images
like Konami-SCC, Ascii-8 and Ascii-16 all mappers for 1Chip-MSX(OCM).

- mglOcm is only for 1chip-MSX compatible loader which loads MSX-Rom image file
needless to change any DIP switches and any mapper patches.

- This is possible because mglOcm use 1chipMSX's hardware mapper controller, if you using mglOcm in
load to rom image will complete supports ASCII8 and ASCII16 mappers
and this executed megarom images perfectly.

SPECIFICATIONS
- full MSX-DOS2 support
- Konami Mapper with SCC
- ASCII 8 kB Mapper
- ASCII 16 kB Mapper
- 2 romimages load to OCM's internal memory slots.

USAGE
- MSXDOS2 must be loaded to run mglOcm.com

Examples:
- a:\roms> mglOcm gradius2.rom
- a:\roms> mglOcm bublbobl.rom

...And more some command line options are as below.

- /o = execute on Konami Classic Mapper
- /s =    on Konami-SCC Mapper
- /8 =    on Ascii-8 Mapper
- /f =    on Ascii16 Mapper
- /l =    on Linear  Mapper
- /r = execute with alternative method
- /t = Z80b 5.37MHz V9958 Fast mode
- /k = Konami 2nd Cartridge secret option
- /j = set Japanese keyboard layout
- /d = back to DOS after loading

REQUIREMENTS
- MSX-DOS2, KdL firmware of v3.1 and over.

CONTACT
- "mglOcm" is written by ToughkidCST
- toughkiddev@gmail.com
