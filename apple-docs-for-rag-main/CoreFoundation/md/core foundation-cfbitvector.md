

- Core Foundation
-  CFBitVector 

Class

# CFBitVector

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFBitVector
```

## Overview

CFBitVector and its derived mutable type, CFMutableBitVector, manage ordered collections of bit values, which are either `0` or `1`. CFBitVector creates static bit vectors and CFMutableBitVector creates dynamic bit vectors.

## Topics

### Creating a Bit Vector

func CFBitVectorCreate(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex) -> CFBitVector!

Creates an immutable bit vector from a block of memory.

func CFBitVectorCreateCopy(CFAllocator!, CFBitVector!) -> CFBitVector!

Creates an immutable bit vector that is a copy of another bit vector.

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

func CFBitVectorGetLastIndexOfBit(CFBitVector!, CFRange, CFBit) -> CFIndex

Locates the last occurrence of a certain bit value within a range of bits in a bit vector.

### Getting the CFBitVector Type ID

func CFBitVectorGetTypeID() -> CFTypeID

Returns the type identifier for the CFBitVector opaque type.

### Data Types

typealias CFBit

A binary value of either `0` or `1`.

## Relationships

### Inherited By

- CFMutableBitVector

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Collections Programming Topics for Core Foundation

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

