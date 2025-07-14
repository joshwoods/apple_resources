

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  readStructure 

# readStructure

``` source
virtual IOReturn readStructure(
 IOMemoryDescriptor *buffer, 
 UInt8format, 
 UInt32address, 
 UInt8layer, 
 UInt8grantID ); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`format`  

As documented by MMC.

`address`  

As documented by MMC.

`layer`  

As documented by MMC.

`grantID`  

As documented by MMC.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC READ DISC STRUCTURE command.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readTrackInfo

reportKey

sendKey

setSpeed

splitTrack

