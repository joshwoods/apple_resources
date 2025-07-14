

- Core Foundation
-  CFMutableSet 

Class

# CFMutableSet

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableSet
```

## Overview

CFMutableSet manages dynamic sets. The basic interface for managing sets is provided by CFSet. CFMutableSet adds functions to modify the contents of a set.

You create a mutable set object using either the CFSetCreateMutable(_:_:_:) or CFSetCreateMutableCopy(_:_:_:) function.

CFMutableSet provides several functions for adding and removing values from a set. The CFSetAddValue(_:_:) function adds a value to a set and CFSetRemoveValue(_:_:) removes a value from a set.

CFMutableSet is “toll-free bridged” with its Cocoa Foundation counterpart, NSMutableSet. What this means is that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. This means that in a method where you see an `NSMutableSet *` parameter, you can pass in a `CFMutableSetRef`, and in a function where you see a `CFMutableSetRef` parameter, you can pass in an NSMutableSet instance. This also applies to concrete subclasses of NSMutableSet. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### CFMutableSet Miscellaneous Functions

func CFSetAddValue(CFMutableSet!, UnsafeRawPointer!)

Adds a value to a CFMutableSet object.

func CFSetCreateMutable(CFAllocator!, CFIndex, UnsafePointer&lt;CFSetCallBacks>!) -> CFMutableSet!

Creates an empty CFMutableSet object.

func CFSetCreateMutableCopy(CFAllocator!, CFIndex, CFSet!) -> CFMutableSet!

Creates a new mutable set with the values from another set.

func CFSetRemoveAllValues(CFMutableSet!)

Removes all values from a CFMutableSet object.

func CFSetRemoveValue(CFMutableSet!, UnsafeRawPointer!)

Removes a value from a CFMutableSet object.

func CFSetReplaceValue(CFMutableSet!, UnsafeRawPointer!)

Replaces a value in a CFMutableSet object.

func CFSetSetValue(CFMutableSet!, UnsafeRawPointer!)

Sets a value in a CFMutableSet object.

## Relationships

### Inherits From

- CFSet

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

