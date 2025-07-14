

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  getSpeed 

# getSpeed

``` source
virtual IOReturn getSpeed(
 UInt16 *kilobytesPerSecond); 
```

## Parameters 

`kilobytesPerSecond`  

Returns the current speed used for data transfers, in kB/s.

kCDSpeedMin specifies the minimum speed for all CD media (1X). kCDSpeedMax specifies the maximum speed supported in hardware.

## Return Value

Returns the status of the operation.

## Overview

Get the current speed used for data transfers.

## See Also

### Miscellaneous

getTOC

read

readCD()

readCD()

readDiscInfo

readISRC

readMCN

readTOC

readTrackInfo

setSpeed

