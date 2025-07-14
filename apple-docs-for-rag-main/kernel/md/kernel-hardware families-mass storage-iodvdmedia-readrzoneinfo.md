

- Kernel
- Hardware Families
- Mass Storage
- IODVDMedia
-  readRZoneInfo 

# readRZoneInfo

``` source
virtual IOReturn readRZoneInfo(
 IOMemoryDescriptor *buffer, 
 UInt32address, 
 DVDRZoneInfoAddressTypeaddressType, 
 UInt16 *actualByteCount ); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`address`  

As documented by MMC.

`addressType`  

As documented by MMC.

`actualByteCount`  

Returns the actual number of bytes transferred in the data transfer.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC READ RZONE INFORMATION (READ TRACK INFORMATION) command.

## See Also

### Miscellaneous

getSpeed

readDiscInfo

readStructure

reportKey

sendKey

setSpeed

