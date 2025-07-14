

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  readTrackInfo 

# readTrackInfo

``` source
virtual IOReturn readTrackInfo(
 IOMemoryDescriptor *buffer, 
 UInt32address, 
 CDTrackInfoAddressTypeaddressType, 
 UInt16 *actualByteCount); 
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

Issue an MMC READ TRACK INFORMATION command.

## See Also

### Miscellaneous

getSpeed

getTOC

read

readCD()

readCD()

readDiscInfo

readISRC

readMCN

readTOC

setSpeed

