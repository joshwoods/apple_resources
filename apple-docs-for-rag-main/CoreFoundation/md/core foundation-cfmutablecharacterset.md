

- Core Foundation
-  CFMutableCharacterSet 

Class

# CFMutableCharacterSet

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class CFMutableCharacterSet
```

## Overview

CFMutableCharacterSet manages dynamic character sets. The basic interface for managing character sets is provided by CFCharacterSet. CFMutableCharacterSet adds functions to modify the contents of a character set.

You create a mutable character set object using either the CFCharacterSetCreateMutable(_:) or CFCharacterSetCreateMutableCopy(_:_:) function.

CFMutableCharacterSet is “toll-free bridged” with its Cocoa Foundation counterpart, NSMutableCharacterSet. This means that the Core Foundation type is interchangeable in function or method calls with the bridged Foundation object. Therefore, in a method where you see an `NSMutableCharacterSet *` parameter, you can pass in a `CFMutableCharacterSetRef`, and in a function where you see a `CFMutableCharacterSetRef` parameter, you can pass in an NSMutableCharacterSet instance. This capability also applies to concrete subclasses of NSMutableCharacterSet. See Toll-Free Bridged Types for more information on toll-free bridging.

## Topics

### Creating a Mutable Character Set

func CFCharacterSetCreateMutable(CFAllocator!) -> CFMutableCharacterSet!

Creates a new empty mutable character set.

func CFCharacterSetCreateMutableCopy(CFAllocator!, CFCharacterSet!) -> CFMutableCharacterSet!

Creates a new mutable character set with the values from another character set.

### Adding Characters

func CFCharacterSetAddCharactersInRange(CFMutableCharacterSet!, CFRange)

Adds a given range to a character set.

func CFCharacterSetAddCharactersInString(CFMutableCharacterSet!, CFString!)

Adds the characters in a given string to a character set.

### Removing Characters

func CFCharacterSetRemoveCharactersInRange(CFMutableCharacterSet!, CFRange)

Removes a given range of Unicode characters from a character set.

func CFCharacterSetRemoveCharactersInString(CFMutableCharacterSet!, CFString!)

Removes the characters in a given string from a character set.

### Logical Operations

func CFCharacterSetIntersect(CFMutableCharacterSet!, CFCharacterSet!)

Forms an intersection of two character sets.

func CFCharacterSetInvert(CFMutableCharacterSet!)

Inverts the content of a given character set.

func CFCharacterSetUnion(CFMutableCharacterSet!, CFCharacterSet!)

Forms the union of two character sets.

## Relationships

### Inherits From

- CFCharacterSet

### Conforms To

- Equatable
- Hashable

## See Also

### Related Documentation

String Programming Guide for Core Foundation

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

