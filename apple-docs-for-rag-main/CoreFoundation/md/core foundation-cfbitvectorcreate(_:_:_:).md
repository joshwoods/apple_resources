

- Core Foundation
-  CFBitVectorCreate(\_:\_:\_:) 

Function

# CFBitVectorCreate(\_:\_:\_:)

Creates an immutable bit vector from a block of memory.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorCreate(
    _ allocator: CFAllocator!,
    _ bytes: UnsafePointer!,
    _ numBits: CFIndex
) -> CFBitVector!
```

## Parameters 

`allocator`  

The allocator to use to allocate memory for the new bit vector. Pass `NULL` or kCFAllocatorDefault to use the current default allocator.

`bytes`  

A pointer to the bit values to store in the new bit vector. The values are copied into the bit vector’s own memory. The bit indices are numbered left-to-right with `0` being the left-most, or most-significant, bit in the byte stream.

`numBits`  

The number of bits in the bit vector.

## Return Value

A new bit vector. Ownership follows the The Create Rule.

## See Also

### Creating a Bit Vector

func CFBitVectorCreateCopy(CFAllocator!, CFBitVector!) -> CFBitVector!

Creates an immutable bit vector that is a copy of another bit vector.

