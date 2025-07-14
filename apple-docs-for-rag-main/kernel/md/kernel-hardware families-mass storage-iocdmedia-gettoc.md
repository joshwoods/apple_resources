

- Kernel
- Hardware Families
- Mass Storage
- IOCDMedia
-  getTOC 

# getTOC

``` source
virtual CDTOC * getTOC(); 
```

## Return Value

Returns a pointer to the TOC buffer (do not deallocate).

## Overview

Get the full Table Of Contents.

All CDTOC fields passed across I/O Kit APIs are guaranteed to be binary-encoded (no BCD-encoded numbers are ever passed).

## See Also

### Miscellaneous

getSpeed

read

readCD()

readCD()

readDiscInfo

readISRC

readMCN

readTOC

readTrackInfo

setSpeed

