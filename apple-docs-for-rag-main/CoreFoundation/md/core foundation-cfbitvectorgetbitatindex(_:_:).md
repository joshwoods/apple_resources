

- Core Foundation
-  CFBitVectorGetBitAtIndex(\_:\_:) 

Function

# CFBitVectorGetBitAtIndex(\_:\_:)

Returns the bit value at a given index in a bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorGetBitAtIndex(
    _ bv: CFBitVector!,
    _ idx: CFIndex
) -> CFBit
```

## Parameters 

`bv`  

The bit vector to examine.

`idx`  

The index of the bit value in `bv` to return.

## Return Value

The bit value at index `idx` in `bv`.

## See Also

### Getting Information About a Bit Vector

func CFBitVectorContainsBit(CFBitVector!, CFRange, CFBit) -> Bool

Returns whether a bit vector contains a particular bit value.

func CFBitVectorGetBits(CFBitVector!, CFRange, UnsafeMutablePointer&lt;UInt8>!)

Returns the bit values in a range of indices in a bit vector.

func CFBitVectorGetCount(CFBitVector!) -> CFIndex

Returns the number of bit values in a bit vector.

func CFBitVectorGetCountOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Counts the number of times a certain bit value occurs within a range of bits in a bit vector.

func CFBitVectorGetFirstIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the first occurrence of a certain bit value within a range of bits in a bit vector.

func CFBitVectorGetLastIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the last occurrence of a certain bit value within a range of bits in a bit vector.

