

- Kernel
- Hardware Families
- Mass Storage
- IODVDMedia
-  getSpeed 

# getSpeed

``` source
virtual IOReturn getSpeed(
 UInt16 *kilobytesPerSecond); 
```

## Parameters 

`kilobytesPerSecond`  

Returns the current speed used for data transfers, in kB/s.

kDVDSpeedMin specifies the minimum speed for all DVD media (1X). kDVDSpeedMax specifies the maximum speed supported in hardware.

## Return Value

Returns the status of the operation.

## Overview

Get the current speed used for data transfers.

## See Also

### Miscellaneous

readDiscInfo

readRZoneInfo

readStructure

reportKey

sendKey

setSpeed

