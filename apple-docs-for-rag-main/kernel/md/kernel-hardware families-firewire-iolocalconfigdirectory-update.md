

- Kernel
- Hardware Families
- FireWire
- IOLocalConfigDirectory
-  update 

# update

``` source
virtual IOReturn update(
 UInt32 offset,
 const UInt32 *&romBase); 
```

## Return Value

kIOReturnSuccess if the specified offset is now accessable at romBase\[offset\].

## Overview

makes sure that the ROM has at least the specified capacity, and that the ROM is uptodate from its start to at least the specified quadlet offset.

