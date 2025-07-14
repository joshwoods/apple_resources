

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  getFragmentCapacity 

# getFragmentCapacity

Accessor to return the number of free fragments in the range.

``` source
virtual UInt32 getFragmentCapacity(
 void ); 
```

## Return Value

Returns the current capacity of free fragment list.

## Overview

This method returns the current capacity of the free fragment list.

## See Also

### Miscellaneous

allocate

Allocates from the free list, at any offset.

allocateRange

Allocates from the free list, at a set offset.

deallocate

Deallocates a range to the free list.

getFragmentCount

Accessor to return the number of free fragments in the range.

getFreeCount

Totals the sizes of the free fragments.

init

Standard initializer for IORangeAllocator.

setFragmentCapacityIncrement

Sets the count of fragments the free list will increase by when full.

withRange

Standard factory method for IORangeAllocator.

