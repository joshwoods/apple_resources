

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  readISRC 

# readISRC

``` source
virtual IOReturn readISRC(
 UInt8track,
 CDISRCisrc); 
```

## Parameters 

`track`  

Track number from which to read the ISRC.

`isrc`  

Buffer for the ISRC data. Buffer contents will be zero-terminated.

## Return Value

Returns the status of the operation.

## Overview

Read the International Standard Recording Code for the specified track.

## See Also

### Miscellaneous

getSpeed

getTOC

read

readCD()

readCD()

readDiscInfo

readMCN

readTOC

readTrackInfo

setSpeed

