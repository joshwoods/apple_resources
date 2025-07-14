

- Core Foundation
-  CFBitVectorFlipBits(\_:\_:) 

Function

# CFBitVectorFlipBits(\_:\_:)

Flips a range of bit values in a bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorFlipBits(
    _ bv: CFMutableBitVector!,
    _ range: CFRange
)
```

## Parameters 

`bv`  

The bit vector to modify.

`range`  

The range of bit values in `bv` to flip. The range must not exceed `0…N-1`, where `N` is the count of the vector.

## See Also

### Related Documentation

func CFBitVectorGetCount(CFBitVector!) -> CFIndex

Returns the number of bit values in a bit vector.

### Modifying a Bit Vector

func CFBitVectorFlipBitAtIndex(CFMutableBitVector!, CFIndex)

Flips a bit value in a bit vector.

func CFBitVectorSetAllBits(CFMutableBitVector!, CFBit)

Sets all bits in a bit vector to a particular value.

func CFBitVectorSetBitAtIndex(CFMutableBitVector!, CFIndex, CFBit)

Sets the value of a particular bit in a bit vector.

func CFBitVectorSetBits(CFMutableBitVector!, CFRange, CFBit)

Sets a range of bits in a bit vector to a particular value.

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

