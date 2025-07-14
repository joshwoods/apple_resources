

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  allocate 

# allocate

Allocates from the free list, at any offset.

``` source
virtual bool allocate(
 IORangeScalar size, 
 IORangeScalar *result, 
 IORangeScalar alignment = 0 ); 
```

## Parameters 

`size`  

The size of the range requested.

`result`  

The beginning of the range allocated is returned here on success.

`alignment`  

If zero is passed, default to the allocators alignment, otherwise pass an alignment required for the allocation, for example 4096 to page align.

## Return Value

Returns true if the allocation was successful, else false.

## Overview

This method allocates a range from the free list. The alignment will default to the alignment set when the allocator was created or may be set here.

## See Also

### Miscellaneous

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

setFragmentCapacityIncrement

Sets the count of fragments the free list will increase by when full.

withRange

Standard factory method for IORangeAllocator.

