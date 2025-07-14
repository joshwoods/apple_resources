

- Kernel
- IOKit Fundamentals
- Memory
-  IORangeAllocator 

Class

# IORangeAllocator

A utility class to manage allocations from a range.

macOS 10.0+

``` source
class IORangeAllocator : OSObject
```

## Overview

The IORangeAllocator class provides functions for allocating ranges, at a fixed or any offset, and freeing them back to a free list. It is useful for describing ranges of memory or address space without requiring storage in the memory - information describing the free elements is kept elsewhere. Ranges are described by a start offset and a size. IORangeAllocator is optionally protected against multithreaded access.

## Topics

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

withRange

Standard factory method for IORangeAllocator.

### Instance Methods

- allocElement

- allocate

- allocateRange

- deallocElement

- deallocate

- free

- getFragmentCapacity

- getFragmentCount

- getFreeCount

- getMetaClass

- init

- serialize

- setFragmentCapacityIncrement

### Type Methods

+ withRange

## Relationships

### Inherits From

- OSObject

## See Also

### Allocation

IOMalloc

Allocates general purpose, wired memory in the kernel map.

IOMallocAligned

Allocates wired memory in the kernel map, with an alignment restriction.

IOMallocPageable

Allocates pageable memory in the kernel map.

IOMallocZero

