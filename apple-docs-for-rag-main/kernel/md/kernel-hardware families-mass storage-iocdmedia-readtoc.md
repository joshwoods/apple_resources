

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  readTOC 

# readTOC

``` source
virtual IOReturn readTOC(
 IOMemoryDescriptor *buffer, 
 CDTOCFormatformat, 
 UInt8formatAsTime, 
 UInt8trackOrSessionNumber, 
 UInt16 *actualByteCount); 
```

## Parameters 

`buffer`  

Buffer for the data transfer. The size of the buffer implies the size of the data transfer.

`format`  

As documented by MMC.

`formatAsTime`  

As documented by MMC.

`trackOrSessionNumber`  

As documented by MMC.

`actualByteCount`  

Returns the actual number of bytes transferred in the data transfer.

## Return Value

Returns the status of the data transfer.

## Overview

Issue an MMC READ TOC/PMA/ATIP command.

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

readTrackInfo

setSpeed

