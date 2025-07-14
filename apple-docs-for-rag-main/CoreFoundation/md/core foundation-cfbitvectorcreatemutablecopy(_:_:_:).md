

- Core Foundation
-  CFBitVectorCreateMutableCopy(\_:\_:\_:) 

Function

# CFBitVectorCreateMutableCopy(\_:\_:\_:)

Creates a new mutable bit vector from a pre-existing bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorCreateMutableCopy(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex,
    _ bv: CFBitVector!
) -> CFMutableBitVector!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new bit vector. The bit vector starts with the same number of values as `bv` and can grow to this number of values (it can have less).

Pass `0` to specify that the maximum capacity is not limited. If non-`0`, `capacity` must be large enough to hold all bit values from `bv`.

`bv`  

The bit vector to copy.

## Return Value

A new bit vector holding the same bit values as `bv`. Ownership follows the The Create Rule

## See Also

### Related Documentation

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

### Creating a CFMutableBitVector Object

func CFBitVectorCreateMutable(CFAllocator!, CFIndex) -> CFMutableBitVector!

Creates a mutable bit vector.

