

- Kernel
- IOKit Fundamentals
- Memory
- IORangeAllocator
-  withRange 

# withRange

Standard factory method for IORangeAllocator.

``` source
static IORangeAllocator * withRange(
 IORangeScalar endOfRange, 
 IORangeScalar defaultAlignment = 0, 
 UInt32 capacity = 0, 
 IOOptionBits options = 0 ); 
```

## Parameters 

`endOfRange`  

If the free list is to contain an initial fragment, set endOfRange to the last offset in the range, ie. size - 1, to create a free fragment for the range zero to endOfRange inclusive. If zero is passed the free list will be initialized empty, and can be populated with calls to the deallocate method.

`defaultAlignment`  

If this parameter is non-zero it specifies a required alignment for all allocations, for example pass 256 to align allocations on 256 byte boundaries. Zero or one specify unaligned allocations.

`capacity`  

Sets the initial size of the free list in number of non-contiguous fragments. This value is also used for the capacityIncrement.

`options`  

Pass kLocking if the instance can be used by multiple threads.

## Return Value

Returns the new IORangeAllocator instance, to be released by the caller, or zero on failure.

## Overview

This method allocates and initializes an IORangeAllocator and optionally sets the free list to contain one fragment, from zero to an endOfRange parameter. The capacity in terms of free fragments and locking options are set for the instance.

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

setFragmentCapacityIncrement

Sets the count of fragments the free list will increase by when full.

