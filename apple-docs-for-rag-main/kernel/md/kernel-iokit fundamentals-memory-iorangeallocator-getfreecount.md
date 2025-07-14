

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  getFreeCount 

# getFreeCount

Totals the sizes of the free fragments.

``` source
virtual IORangeScalar getFreeCount(
 void ); 
```

## Return Value

Returns the total of the free fragments sizes.

## Overview

This method returns the total of the sizes of the fragments on the free list.

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

getFragmentCount

Accessor to return the number of free fragments in the range.

init

Standard initializer for IORangeAllocator.

setFragmentCapacityIncrement

Sets the count of fragments the free list will increase by when full.

withRange

Standard factory method for IORangeAllocator.

