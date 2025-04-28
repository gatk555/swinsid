Here are new firmware files for Swinsid devices based on the modified
source code in this repository.

Lazy_Jones_20250428.hex
Swinkels_20240528.hex

Built from modified versions of Daniël Mantione's source code.  The "low-hanging fruit" has been plucked.  That includes code in sample generation that blends the current value from table lookup with the previous output and an intermediate sample.  The cycle controlling byte, that controls pitch, is now loaded
from a Flash location and set to 98, calculated for PAL.  For NTSC, edit the penultimate line of the hex file, changing :011C00006281 to :011C00005E85.

