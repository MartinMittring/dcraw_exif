# dcraw_exif
This project is not part of UnrealEngine but it was used for the UnrealEngine Kite demo. See:
  https://www.youtube.com/watch?v=_zVddsYKZnw
  https://www.youtube.com/watch?v=clakekAHQx0

The code was tested with multiple Canon cameras using the .CR2 (raw) format as input.

Typical commandline:
  dcraw -4 -w -o 1 -T -Z 18 15 -n 100 MyPath/MyImage.CR2

* -4 => Linear 16-bit
* -w => use camera white balance
* -o 1 => sRGB (?? is that right?)
* -T => Write TIFF
* -Z 18 15 => crop the borders like Canon would do it to get the same sized image
* -n 100 => fixes noise in the darks

Compile with Visual Studio 2012:
* Create new console application
* add dcraw.c
* compile (some warnings are not fixed yet)

History:
* 4/22/2015 MM Started with original from: https://www.cybercom.net/~dcoffin/dcraw/dcraw.c
* 4/22/2015 MM Updated with changes from Rob Sumner: https://users.soe.ucsc.edu/~rcsumner/rawguide/dcraw_win.c
* 4/22/2015 MM added new features: crop and downsample


