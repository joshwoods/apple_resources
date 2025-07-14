

- Core Foundation
-  CFBitVectorGetBits(\_:\_:\_:) 

Function

# CFBitVectorGetBits(\_:\_:\_:)

Returns the bit values in a range of indices in a bit vector.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBitVectorGetBits(
    _ bv: CFBitVector!,
    _ range: CFRange,
    _ bytes: UnsafeMutablePointer!
)
```

## Parameters 

`bv`  

The bit vector to examine.

`range`  

The range of bit values to return.

`bytes`  

On return, contains the requested bit values from `bv`. This argument must point to enough memory to hold the number of bits requested. The requested bits are left-aligned with the first requested bit stored in the left-most, or most-significant, bit of the byte stream.

## See Also

### Getting Information About a Bit Vector

func CFBitVectorContainsBit(CFBitVector!, CFRange, CFBit) -> Bool

Returns whether a bit vector contains a particular bit value.

func CFBitVectorGetBitAtIndex(CFBitVector!, CFIndex) -> CFBit

Returns the bit value at a given index in a bit vector.

func CFBitVectorGetCount(CFBitVector!) -> CFIndex

Returns the number of bit values in a bit vector.

func CFBitVectorGetCountOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Counts the number of times a certain bit value occurs within a range of bits in a bit vector.

func CFBitVectorGetFirstIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the first occurrence of a certain bit value within a range of bits in a bit vector.

func CFBitVectorGetLastIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the last occurrence of a certain bit value within a range of bits in a bit vector.

