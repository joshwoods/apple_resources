

- Kernel
- Hardware Families
- Mass Storage
- IOBDMedia
-  sendKey 

# sendKey

``` source
virtual IOReturn sendKey(
 IOMemoryDescriptor *buffer, 
 UInt8keyClass, 
 UInt8grantID, 
 UInt8format ); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`keyClass`  

As documented by MMC.

`grantID`  

As documented by MMC.

`format`  

As documented by MMC.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC SEND KEY command.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readStructure

readTrackInfo

reportKey

setSpeed

splitTrack

