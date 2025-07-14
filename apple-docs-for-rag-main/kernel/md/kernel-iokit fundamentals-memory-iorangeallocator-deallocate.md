

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  deallocate 

# deallocate

Deallocates a range to the free list.

``` source
virtual void deallocate(
 IORangeScalarstart, 
 IORangeScalarsize ); 
```

## Parameters 

`start`  

The beginning of the range requested.

`size`  

Returns the size of the range requested.

## Overview

This method deallocates a range to the free list, given a the start offset and length passed in.

## See Also

### Miscellaneous

allocate

Allocates from the free list, at any offset.

allocateRange

Allocates from the free list, at a set offset.

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

