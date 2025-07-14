

- Kernel
- IOKit Fundamentals
- Memory
- IOMemoryDescriptor
-  getLength 

# getLength

Accessor to get the length of the memory descriptor (over all its ranges).

``` source
virtual IOByteCount getLength() const; 
```

## Return Value

The byte count.

## Overview

This method returns the total length of the memory described by the descriptor, ie. the sum of its ranges' lengths.

## See Also

### Getting the Descriptor Information

getDirection

Gets the direction of memory transfers associated with the descriptor.

- getDirection

Gets the direction of memory transfers associated with the descriptor.

- getLength

Accessor to get the length of the memory descriptor (over all its ranges).

- GetLength

Returns the length of the memory block represented by this object.

- getDMAMapLength

- getFlags

Returns the options used to create the memory descriptor.

- getMetaClass

