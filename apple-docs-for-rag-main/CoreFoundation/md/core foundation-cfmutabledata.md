

- Core Foundation
-  CFMutableData 

Class

# CFMutableData

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableData
```

## Overview

CFMutableData manages dynamic binary data. The basic interface for managing binary data is provided by CFData. CFMutableData adds functions to modify the contents of a binary data object.

You create a mutable data object using either the CFDataCreateMutable(_:_:) or CFDataCreateMutableCopy(_:_:_:) function.

Bytes are added to a data object with the CFDataAppendBytes(_:_:_:) function. Bytes are removed from a data object with the CFDataDeleteBytes(_:_:) function.

Important

Many of the CFMutableData functions take a CFIndex `length` or `capacity` argument. You must not pass a negative number for such values—this may introduce a security risk.

CFMutableData is “toll-free bridged” with its Cocoa Foundation counterpart, NSMutableData. What this means is that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. In other words, in a method where you see an `NSMutableData *` parameter, you can pass in a `CFMutableDataRef`, and in a function where you see a `CFMutableDataRef` parameter, you can pass in an `NSMutableData` instance. This also applies to concrete subclasses of `NSMutableData`. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating a Mutable Data Object

func CFDataCreateMutable(CFAllocator!, CFIndex) -> CFMutableData!

Creates an empty CFMutableData object.

func CFDataCreateMutableCopy(CFAllocator!, CFIndex, CFData!) -> CFMutableData!

Creates a CFMutableData object by copying another CFData object.

### Accessing Data

func CFDataGetMutableBytePtr(CFMutableData!) -> UnsafeMutablePointer&lt;UInt8>!

Returns a pointer to a mutable byte buffer of a CFMutableData object.

### Modifying a Mutable Data Object

func CFDataAppendBytes(CFMutableData!, UnsafePointer&lt;UInt8>!, CFIndex)

Appends the bytes from a byte buffer to the contents of a CFData object.

func CFDataDeleteBytes(CFMutableData!, CFRange)

Deletes the bytes in a CFMutableData object within a specified range.

func CFDataReplaceBytes(CFMutableData!, CFRange, UnsafePointer&lt;UInt8>!, CFIndex)

Replaces those bytes in a CFMutableData object that fall within a specified range with other bytes.

func CFDataIncreaseLength(CFMutableData!, CFIndex)

Increases the length of a CFMutableData object’s internal byte buffer, zero-filling the extension to the buffer.

func CFDataSetLength(CFMutableData!, CFIndex)

Resets the length of a CFMutableData object’s internal byte buffer.

## Relationships

### Inherits From

- CFData

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

Property List Programming Topics for Core Foundation

Binary Data Programming Guide for Core Foundation

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

