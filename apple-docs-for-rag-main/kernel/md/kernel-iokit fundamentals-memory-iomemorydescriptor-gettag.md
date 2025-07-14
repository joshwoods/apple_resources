

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  getTag 

# getTag

Accessor to the retrieve the tag for the memory descriptor.

``` source
virtual IOOptionBits getTag(
 void ); 
```

## Return Value

The tag.

## Overview

This method returns the tag for the memory descriptor. Tag bits are not interpreted by IOMemoryDescriptor.

## See Also

### Accessing the Buffer's Tag

- getTag

Accessor to the retrieve the tag for the memory descriptor.

setTag

Set the tag for the memory descriptor.

- setTag

Set the tag for the memory descriptor.

- getVMTag

- setVMTags

