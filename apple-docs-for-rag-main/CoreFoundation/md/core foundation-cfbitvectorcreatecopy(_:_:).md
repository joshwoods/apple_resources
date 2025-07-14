

- Core Foundation
-  CFBitVectorCreateCopy(\_:\_:) 

Function

# CFBitVectorCreateCopy(\_:\_:)

Creates an immutable bit vector that is a copy of another bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorCreateCopy(
    _ allocator: CFAllocator!,
    _ bv: CFBitVector!
) -> CFBitVector!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new bit vector. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bv`  

The bit vector to copy.

## Return Value

A new bit vector holding the same bit values as `bv`. Ownership follows the The Create Rule.

## See Also

### Creating a Bit Vector

func CFBitVectorCreate(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex) -> CFBitVector!

Creates an immutable bit vector from a block of memory.

