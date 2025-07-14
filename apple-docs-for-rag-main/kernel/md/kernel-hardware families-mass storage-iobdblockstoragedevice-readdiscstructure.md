

- Kernel
- Hardware Families
- Mass Storage
- IOBDBlockStorageDevice
-  readDiscStructure 

# readDiscStructure

``` source
virtual IOReturn readDiscStructure(
 IOMemoryDescriptor *buffer, 
 UInt8format, 
 UInt32address, 
 UInt8layer, 
 UInt8grantID, 
 UInt8type ) = 0; 
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

`type`  

As documented by MMC.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC READ DISC STRUCTURE command.

## See Also

### Miscellaneous

init

splitTrack

