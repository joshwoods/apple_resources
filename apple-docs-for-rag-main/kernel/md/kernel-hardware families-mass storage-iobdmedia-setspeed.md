

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  setSpeed 

# setSpeed

``` source
virtual IOReturn setSpeed(
 UInt16kilobytesPerSecond); 
```

## Parameters 

`kilobytesPerSecond`  

Speed to be used for data transfers, in kB/s.

kBDSpeedMin specifies the minimum speed for all BD media (1X). kBDSpeedMax specifies the maximum speed supported in hardware.

## Return Value

Returns the status of the operation.

## Overview

Set the speed to be used for data transfers.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readStructure

readTrackInfo

reportKey

sendKey

splitTrack

