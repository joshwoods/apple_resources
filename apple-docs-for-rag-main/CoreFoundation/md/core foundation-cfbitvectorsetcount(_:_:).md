

- Core Foundation
-  CFBitVectorSetCount(\_:\_:) 

Function

# CFBitVectorSetCount(\_:\_:)

Changes the size of a mutable bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorSetCount(
    _ bv: CFMutableBitVector!,
    _ count: CFIndex
)
```

## Parameters 

`bv`  

The bit vector to modify.

`count`  

The new size for `bv`. If `count` is greater than the current size of `bv`, the additional bit values are set to `0`.

## Discussion

If `bv` was created with a fixed capacity, you cannot increase its size beyond that capacity.

## See Also

### Related Documentation

func CFBitVectorCreateMutable(CFAllocator!, CFIndex) -> CFMutableBitVector!

Creates a mutable bit vector.

func CFBitVectorCreateMutableCopy(CFAllocator!, CFIndex, CFBitVector!) -> CFMutableBitVector!

Creates a new mutable bit vector from a pre-existing bit vector.

func CFBitVectorGetCount(CFBitVector!) -> CFIndex

Returns the number of bit values in a bit vector.

### Modifying a Bit Vector

func CFBitVectorFlipBitAtIndex(CFMutableBitVector!, CFIndex)

Flips a bit value in a bit vector.

func CFBitVectorFlipBits(CFMutableBitVector!, CFRange)

Flips a range of bit values in a bit vector.

func CFBitVectorSetAllBits(CFMutableBitVector!, CFBit)

Sets all bits in a bit vector to a particular value.

func CFBitVectorSetBitAtIndex(CFMutableBitVector!, CFIndex, CFBit)

Sets the value of a particular bit in a bit vector.

func CFBitVectorSetBits(CFMutableBitVector!, CFRange, CFBit)

Sets a range of bits in a bit vector to a particular value.

