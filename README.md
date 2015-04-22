# dcraw_exif
mirror of https://www.cybercom.net/~dcoffin/dcraw with updates, additionally maintain exif data


This project is not part of UnrealEngine but it was used for the UnrealEngine Kite demo. See:
  https://www.youtube.com/watch?v=_zVddsYKZnw
  https://www.youtube.com/watch?v=clakekAHQx0

The code was tested with multiple Canon cameras using the .CRW (raw) format as input.

Typical commandline settings:
  dcraw -4 -w -o 1 -T -Z 18 15 -n 100 MyPath/MyImage.CR2

History:
* 4/22/2015 MM Started with original from: https://www.cybercom.net/~dcoffin/dcraw/dcraw.c
* 4/22/2015 MM Updated with changes from Rob Sumner: https://users.soe.ucsc.edu/~rcsumner/rawguide/dcraw_win.c
* 4/22/2015 MM added new features: crop and downsample


