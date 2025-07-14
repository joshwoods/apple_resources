

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  allocateRange 

# allocateRange

Allocates from the free list, at a set offset.

``` source
virtual bool allocateRange(
 IORangeScalarstart, 
 IORangeScalarsize ); 
```

## Parameters 

`start`  

The beginning of the range requested.

`size`  

The size of the range requested.

## Return Value

Returns true if the allocation was successful, else false.

## Overview

This method allocates a range from the free list, given a set offset passed in.

## See Also

### Miscellaneous

allocate

Allocates from the free list, at any offset.

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

