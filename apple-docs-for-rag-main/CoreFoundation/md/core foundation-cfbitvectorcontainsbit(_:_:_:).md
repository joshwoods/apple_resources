

- Core Foundation
-  CFBitVectorContainsBit(\_:\_:\_:) 

Function

# CFBitVectorContainsBit(\_:\_:\_:)

Returns whether a bit vector contains a particular bit value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorContainsBit(
    _ bv: CFBitVector!,
    _ range: CFRange,
    _ value: CFBit
) -> Bool
```

## Parameters 

`bv`  

The bit vector to search.

`range`  

The range of bits in `bv` to search.

`value`  

The bit value for which to search.

## Return Value

`true` if the specified range of bits in `bv` contains `value`, otherwise `false`.

## See Also

### Getting Information About a Bit Vector

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

func CFBitVectorGetLastIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the last occurrence of a certain bit value within a range of bits in a bit vector.

