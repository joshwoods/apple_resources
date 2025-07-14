

- Core Foundation
-  CFData 

Class

# CFData

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFData
```

## Overview

CFData and its derived mutable type, CFMutableData, provide support for data objects, object-oriented wrappers for byte buffers. Data objects let simple allocated buffers (that is, data with no embedded pointers) take on the behavior of Core Foundation objects. CFData creates static data objects, and CFMutableData creates dynamic data objects. Data objects are typically used for raw data storage.

You use the CFDataCreate(_:_:_:) and CFDataCreateCopy(_:_:) functions to create static data objects. These functions make a new copy of the supplied data. To create a data object that uses the supplied buffer instead of making a separate copy, use the CFDataCreateWithBytesNoCopy(_:_:_:_:) function. You use the CFDataGetBytes(_:_:_:) function to retrieve the bytes and the CFDataGetLength(_:) function to get the length of the bytes.

CFData is “toll-free bridged” with its Cocoa Foundation counterpart, NSData. What this means is that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. In other words, in a method where you see an `NSData *` parameter, you can pass in a `CFDataRef`, and in a function where you see a `CFDataRef` parameter, you can pass in an `NSData` instance. This also applies to concrete subclasses of `NSData`. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating a CFData Object

func CFDataCreate(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex) -> CFData!

Creates an immutable CFData object using data copied from a specified byte buffer.

func CFDataCreateCopy(CFAllocator!, CFData!) -> CFData!

Creates an immutable copy of a CFData object.

func CFDataCreateWithBytesNoCopy(CFAllocator!, UnsafePointer&lt;UInt8>!, CFIndex, CFAllocator!) -> CFData!

Creates an immutable CFData object from an external (client-owned) byte buffer.

### Examining a CFData Object

func CFDataGetBytePtr(CFData!) -> UnsafePointer&lt;UInt8>!

Returns a read-only pointer to the bytes of a CFData object.

func CFDataGetBytes(CFData!, CFRange, UnsafeMutablePointer&lt;UInt8>!)

Copies the byte contents of a CFData object to an external buffer.

func CFDataGetLength(CFData!) -> CFIndex

Returns the number of bytes contained by a CFData object.

func CFDataFind(CFData!, CFData!, CFRange, CFDataSearchFlags) -> CFRange

Finds and returns the range within a data object of the first occurrence of the given data, within a given range, subject to any given options.

### Getting the CFData Type ID

func CFDataGetTypeID() -> CFTypeID

Returns the type identifier for the CFData opaque type.

### Data Types

struct CFDataSearchFlags

A CFOptionFlags type for specifying options for searching.

## Relationships

### Inherited By

- CFMutableData

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

class CFDate

class CFDateFormatter

class CFDictionary

class CFError

class CFFileDescriptor

