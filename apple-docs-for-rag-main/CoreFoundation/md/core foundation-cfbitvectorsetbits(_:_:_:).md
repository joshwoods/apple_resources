

- Core Foundation
-  CFBitVectorSetBits(\_:\_:\_:) 

Function

# CFBitVectorSetBits(\_:\_:\_:)

Sets a range of bits in a bit vector to a particular value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorSetBits(
    _ bv: CFMutableBitVector!,
    _ range: CFRange,
    _ value: CFBit
)
```

## Parameters 

`bv`  

The bit vector to modify.

`range`  

The range of bits to set. The range must not exceed `0…N-1`, where `N` is the count of the vector.

`value`  

The bit value to which to set the range of bits.

## See Also

### Related Documentation

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

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

