

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  splitTrack 

# splitTrack

``` source
virtual IOReturn splitTrack(
 UInt32address); 
```

## Parameters 

`address`  

As documented by MMC.

## Return Value

Returns the status of the operation.

## Overview

Issue an MMC RESERVE TRACK command with the ARSV bit.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readStructure

readTrackInfo

reportKey

sendKey

setSpeed

