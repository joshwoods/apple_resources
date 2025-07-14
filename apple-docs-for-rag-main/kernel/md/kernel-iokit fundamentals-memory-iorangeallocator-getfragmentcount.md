

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  getFragmentCount 

# getFragmentCount

Accessor to return the number of free fragments in the range.

``` source
virtual UInt32 getFragmentCount(
 void ); 
```

## Return Value

Returns the count of free fragments.

## Overview

This method returns a count of free fragments. Each fragment describes a non-contiguous free range - deallocations will merge contiguous fragments together.

## See Also

### Miscellaneous

allocate

Allocates from the free list, at any offset.

allocateRange

Allocates from the free list, at a set offset.

deallocate

Deallocates a range to the free list.

getFragmentCapacity

Accessor to return the number of free fragments in the range.

getFreeCount

Totals the sizes of the free fragments.

init

Standard initializer for IORangeAllocator.

setFragmentCapacityIncrement

Sets the count of fragments the free list will increase by when full.

withRange

Standard factory method for IORangeAllocator.

