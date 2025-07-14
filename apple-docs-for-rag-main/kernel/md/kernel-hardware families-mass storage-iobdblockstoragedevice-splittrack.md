

- Kernel
- Hardware Families
- Mass Storage
- IOBDBlockStorageDevice
-  splitTrack 

# splitTrack

``` source
virtual IOReturn splitTrack(
 UInt32address) = 0; 
```

## Parameters 

`address`  

As documented by MMC.

## Return Value

Returns the status of the operation.

## Overview

Issue an MMC RESERVE TRACK command with the ARSV bit.

## See Also

### Miscellaneous

init

readDiscStructure

