

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  readTrackInfo 

# readTrackInfo

``` source
virtual IOReturn readTrackInfo(
 IOMemoryDescriptor *buffer, 
 UInt32address, 
 UInt8addressType, 
 UInt8open, 
 UInt16 *actualByteCount ); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`address`  

As documented by MMC.

`addressType`  

As documented by MMC.

`open`  

Reserved for future use. Set to zero.

`actualByteCount`  

Returns the actual number of bytes transferred in the data transfer.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC READ TRACK INFORMATION command.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readStructure

reportKey

sendKey

setSpeed

splitTrack

