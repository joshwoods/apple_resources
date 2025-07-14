

- Core Foundation
-  CFMutableBitVector 

Class

# CFMutableBitVector

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableBitVector
```

## Overview

CFMutableBitVector objects manage dynamic bit vectors. The basic interface for managing bit vectors is provided by CFBitVector. CFMutableBitVector adds functions to modify the contents of a bit vector.

You create a mutable bit vector object using either the CFBitVectorCreateMutable(_:_:) or CFBitVectorCreateMutableCopy(_:_:_:) function. You add to and remove from a bit vector by altering the size of the bit vector with the CFBitVectorSetCount(_:_:) function

## Topics

### Creating a CFMutableBitVector Object

func CFBitVectorCreateMutable(CFAllocator!, CFIndex) -> CFMutableBitVector!

Creates a mutable bit vector.

func CFBitVectorCreateMutableCopy(CFAllocator!, CFIndex, CFBitVector!) -> CFMutableBitVector!

Creates a new mutable bit vector from a pre-existing bit vector.

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

func CFBitVectorSetCount(CFMutableBitVector!, CFIndex)

Changes the size of a mutable bit vector.

## Relationships

### Inherits From

- CFBitVector

### Conforms To

- Equatable
- Hashable

## See Also

### Opaque Types

class CFAllocator

class CFArray

class CFAttributedString

class CFBag

class CFBinaryHeap

class CFBitVector

class CFBoolean

class CFBundle

class CFCalendar

class CFCharacterSet

class CFData

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

