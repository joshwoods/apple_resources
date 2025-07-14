

- Kernel
- Hardware Families
- Mass Storage
- IODVDMedia
-  sendKey 

# sendKey

``` source
virtual IOReturn sendKey(
 IOMemoryDescriptor *buffer, 
 const DVDKeyClasskeyClass, 
 const UInt8grantID, 
 const DVDKeyFormatformat ); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer. Pass null for the kDVDKeyFormatAGID_Invalidate format case.

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

readRZoneInfo

readStructure

reportKey

setSpeed

