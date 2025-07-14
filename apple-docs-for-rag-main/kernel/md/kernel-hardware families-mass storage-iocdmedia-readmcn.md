

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  readMCN 

# readMCN

``` source
virtual IOReturn readMCN(
 CDMCNmcn); 
```

## Parameters 

`mcn`  

Buffer for the MCN data. Buffer contents will be zero-terminated.

## Return Value

Returns the status of the operation.

## Overview

Read the Media Catalog Number (also known as the Universal Product Code).

## See Also

### Miscellaneous

getSpeed

getTOC

read

readCD()

readCD()

readDiscInfo

readISRC

readTOC

readTrackInfo

setSpeed

