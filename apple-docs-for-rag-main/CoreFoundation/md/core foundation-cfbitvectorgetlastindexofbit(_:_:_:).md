

- Core Foundation
-  CFBitVectorGetLastIndexOfBit(\_:\_:\_:) 

Function

# CFBitVectorGetLastIndexOfBit(\_:\_:\_:)

Locates the last occurrence of a certain bit value within a range of bits in a bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorGetLastIndexOfBit(
    _ bv: CFBitVector!,
    _ range: CFRange,
    _ value: CFBit
) -> CFIndex
```

## Parameters 

`bv`  

The bit vector to examine.

`range`  

The range of bits in `bv` to search.

`value`  

The bit value for which to search.

## Return Value

The index of the last occurrence of `value` in the specified range of `bv`, or `kCFNotFound` if `value` is not present.

## See Also

### Getting Information About a Bit Vector

func CFBitVectorContainsBit(CFBitVector!, CFRange, CFBit) -> Bool

Returns whether a bit vector contains a particular bit value.

func CFBitVectorGetBitAtIndex(CFBitVector!, CFIndex) -> CFBit

Returns the bit value at a given index in a bit vector.

func CFBitVectorGetBits(CFBitVector!, CFRange, UnsafeMutablePointer&lt;UInt8>!)

Returns the bit values in a range of indices in a bit vector.

func CFBitVectorGetCount(CFBitVector!) -> CFIndex

Returns the number of bit values in a bit vector.

func CFBitVectorGetCountOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Counts the number of times a certain bit value occurs within a range of bits in a bit vector.

func CFBitVectorGetFirstIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the first occurrence of a certain bit value within a range of bits in a bit vector.

