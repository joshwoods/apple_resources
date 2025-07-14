

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  setFragmentCapacityIncrement 

# setFragmentCapacityIncrement

Sets the count of fragments the free list will increase by when full.

``` source
virtual void setFragmentCapacityIncrement(
 UInt32count ); 
```

## Parameters 

`count`  

The number of fragments to increment the capacity by when the free list is full.

## Overview

This method sets the number of extra fragments the free list will expand to when full. It defaults to the initial capacity.

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

getFreeCount

Totals the sizes of the free fragments.

init

Standard initializer for IORangeAllocator.

withRange

Standard factory method for IORangeAllocator.

