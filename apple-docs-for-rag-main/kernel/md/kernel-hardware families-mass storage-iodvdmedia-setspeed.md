

- Kernel
- Hardware Families
- Mass Storage
- IODVDMedia
-  setSpeed 

# setSpeed

``` source
virtual IOReturn setSpeed(
 UInt16kilobytesPerSecond); 
```

## Parameters 

`kilobytesPerSecond`  

Speed to be used for data transfers, in kB/s.

kDVDSpeedMin specifies the minimum speed for all DVD media (1X). kDVDSpeedMax specifies the maximum speed supported in hardware.

## Return Value

Returns the status of the operation.

## Overview

Set the speed to be used for data transfers.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readRZoneInfo

readStructure

reportKey

sendKey

