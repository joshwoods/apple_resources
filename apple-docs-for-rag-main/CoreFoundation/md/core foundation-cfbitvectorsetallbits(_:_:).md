

- Core Foundation
-  CFBitVectorSetAllBits(\_:\_:) 

Function

# CFBitVectorSetAllBits(\_:\_:)

Sets all bits in a bit vector to a particular value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorSetAllBits(
    _ bv: CFMutableBitVector!,
    _ value: CFBit
)
```

## Parameters 

`bv`  

The bit vector to modify.

`value`  

The bit value to which to set all bits in `bv`.

## See Also

### Modifying a Bit Vector

func CFBitVectorFlipBitAtIndex(CFMutableBitVector!, CFIndex)

Flips a bit value in a bit vector.

func CFBitVectorFlipBits(CFMutableBitVector!, CFRange)

Flips a range of bit values in a bit vector.

func CFBitVectorSetBitAtIndex(CFMutableBitVector!, CFIndex, CFBit)

Sets the value of a particular bit in a bit vector.

func CFBitVectorSetBits(CFMutableBitVector!, CFRange, CFBit)

Sets a range of bits in a bit vector to a particular value.

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

