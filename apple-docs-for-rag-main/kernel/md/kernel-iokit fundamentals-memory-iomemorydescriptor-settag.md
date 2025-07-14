

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  setTag 

# setTag

Set the tag for the memory descriptor.

``` source
virtual void setTag(
 IOOptionBitstag ); 
```

## Parameters 

`tag`  

The tag.

## Overview

This method sets the tag for the memory descriptor. Tag bits are not interpreted by IOMemoryDescriptor.

## See Also

### Accessing the Buffer's Tag

getTag

Accessor to the retrieve the tag for the memory descriptor.

- getTag

Accessor to the retrieve the tag for the memory descriptor.

- setTag

Set the tag for the memory descriptor.

- getVMTag

- setVMTags

