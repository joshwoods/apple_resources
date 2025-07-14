

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  readDiscInfo 

# readDiscInfo

``` source
virtual IOReturn readDiscInfo(
 IOMemoryDescriptor *buffer, 
 UInt8type, 
 UInt16 *actualByteCount ); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`type`  

Reserved for future use. Set to zero.

`actualByteCount`  

Returns the actual number of bytes transferred in the data transfer.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC READ DISC INFORMATION command.

## See Also

### Miscellaneous

getSpeed

readStructure

readTrackInfo

reportKey

sendKey

setSpeed

splitTrack

