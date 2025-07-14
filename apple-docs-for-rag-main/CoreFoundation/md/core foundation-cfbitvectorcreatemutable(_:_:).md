

- Core Foundation
-  CFBitVectorCreateMutable(\_:\_:) 

Function

# CFBitVectorCreateMutable(\_:\_:)

Creates a mutable bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorCreateMutable(
    _ allocator: CFAllocator!,
    _ capacity: CFIndex
) -> CFMutableBitVector!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new object. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`capacity`  

The maximum number of values that can be contained by the new bit vector. The bit vector starts empty and can grow to this number of values (and it can have less).

Pass `0` to specify that the maximum capacity is not limited. The value must not be negative.

## Return Value

A new bit vector. Ownership follows the The Create Rule.

## See Also

### Related Documentation

Collections Programming Topics for Core Foundation

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

### Creating a CFMutableBitVector Object

func CFBitVectorCreateMutableCopy(CFAllocator!, CFIndex, CFBitVector!) -> CFMutableBitVector!

Creates a new mutable bit vector from a pre-existing bit vector.

