

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  getSpeed 

# getSpeed

``` source
virtual IOReturn getSpeed(
 UInt16 *kilobytesPerSecond); 
```

## Parameters 

`kilobytesPerSecond`  

Returns the current speed used for data transfers, in kB/s.

kBDSpeedMin specifies the minimum speed for all BD media (1X). kBDSpeedMax specifies the maximum speed supported in hardware.

## Return Value

Returns the status of the operation.

## Overview

Get the current speed used for data transfers.

## See Also

### Miscellaneous

readDiscInfo

readStructure

readTrackInfo

reportKey

sendKey

setSpeed

splitTrack

