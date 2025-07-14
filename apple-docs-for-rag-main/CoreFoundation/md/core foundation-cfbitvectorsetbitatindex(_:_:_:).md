

- Core Foundation
-  CFBitVectorSetBitAtIndex(\_:\_:\_:) 

Function

# CFBitVectorSetBitAtIndex(\_:\_:\_:)

Sets the value of a particular bit in a bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorSetBitAtIndex(
    _ bv: CFMutableBitVector!,
    _ idx: CFIndex,
    _ value: CFBit
)
```

## Parameters 

`bv`  

The bit vector to modify.

`idx`  

The index of the bit value to set. The index must be in the range `0…N-1`, where `N` is the count of the vector.

`value`  

The bit value to which to set the bit at index `idx`.

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

func CFBitVectorSetBits(CFMutableBitVector!, CFRange, CFBit)

Sets a range of bits in a bit vector to a particular value.

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

