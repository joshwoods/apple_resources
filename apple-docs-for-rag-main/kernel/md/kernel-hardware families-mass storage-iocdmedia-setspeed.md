

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  setSpeed 

# setSpeed

``` source
virtual IOReturn setSpeed(
 UInt16kilobytesPerSecond); 
```

## Parameters 

`kilobytesPerSecond`  

Speed to be used for data transfers, in kB/s.

kCDSpeedMin specifies the minimum speed for all CD media (1X). kCDSpeedMax specifies the maximum speed supported in hardware.

## Return Value

Returns the status of the operation.

## Overview

Set the speed to be used for data transfers.

## See Also

### Miscellaneous

getSpeed

getTOC

read

readCD()

readCD()

readDiscInfo

readISRC

readMCN

readTOC

readTrackInfo

